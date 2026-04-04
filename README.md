# KH1 ARD & EVDL Editor

A lightweight web-based toolset for editing **ARD (map/entity data)** and **EVDL (event/script logic)** files used in *Kingdom Hearts I*. Made by gg3502

---

## Features

### ARD Editor (Entity / Map Data)

The ARD editor allows you to create and modify in-game objects and their properties.

#### Core Functionality
- Add / clone entities (NPCs, treasure chests, objects)
- Edit:
  - Entity ID (`Set_char_ID`)
  - Position (X / Z coordinates)
  - Rotation / orientation
  - Flags & parameters
- Duplicate existing objects for fast testing

#### What ARD Controls
- What objects exist in the room  
- Where they are placed  
- Targeting / interaction availability  

> If an object is not in ARD, EVDL cannot control it.
> 

### EVDL Editor (Event / Script Logic)

The EVDL editor allows you to modify object behavior using BDX-style scripting.

#### Core Functionality
- Edit opcodes:
  - `push`
  - `syscall`
  - `alu`
  - `beqz`, `jmp`
- Build custom interaction logic
- Control:
  - Messages
  - Animations
  - Event mode
  - Object visibility / collision

#### What EVDL Controls
- What happens when interacting with objects  
- Event flow (messages, cutscenes)  
- Object behavior (show/hide, effects)



## ARD vs EVDL

| System | Purpose |
|--------|--------|
| **ARD** | Defines the object |
| **EVDL** | Defines what it does |

### Example Workflow

1. **ARD**
   - Spawn chest entity
   - Enable targeting

2. **EVDL**
   - Handle interaction
   - Give item / show message
   - Hide chest after use

---

## Notes & Quirks

- Coordinates use **X/Z plane**
- Y position is handled automatically by the engine
- Values may be interpreted as **floats internally**
- Some scripts split values.

## Example Script (EVDL)

Below is a real example of a EVDL script that continuously scales an object up and down:

```asm
[ 7960]  1F000909  push            0x9001F           ; 589855
[ 7961]  0A000018  syscall         10                ; Set_char_ID
[ 7962]  10000005  yield           0x10            

[ 7963]  C8000009  push            0xC8              ; 200
[ 7964]  C8000009  push            0xC8              ; 200
[ 7965]  C8000009  push            0xC8              ; 200
[ 7966]  C8000009  push            0xC8              ; 200
[ 7967]  78000009  push            0x78              ; 120
[ 7968]  7A000018  syscall         122               ; Change_char_scale

[ 7969]  78000009  push            0x78              ; 120
[ 7970]  08000018  syscall         8                 ; Set_wait_timer

[ 7971]  32000009  push            0x32              ; 50
[ 7972]  32000009  push            0x32              ; 50
[ 7973]  32000009  push            0x32              ; 50
[ 7974]  32000009  push            0x32              ; 50
[ 7975]  78000009  push            0x78              ; 120
[ 7976]  7A000018  syscall         122               ; Change_char_scale

[ 7977]  78000009  push            0x78              ; 120
[ 7978]  08000018  syscall         8                 ; Set_wait_timer

[ 7979]  F0FFFF02  jmp             -16               ; → PC 7963
```


Below is another real example of a EVDL script that opens message when reaction command is pressed:

```asm

  [ 2528]  07000409  push            0x40007           ; 262151
  [ 2529]  0A000018  syscall         10                ; Set_char_ID
  [ 2530]  96000009  push            0x96              ; 150
  [ 2531]  C7000018  syscall         199               ; Set_command_check_range
  [ 2532]  10000005  yield           0x10            
  [ 2533]  01000009  push            0x1             
  [ 2534]  02000003  beqz            +2                ; → PC 2536
  [ 2535]  FEFFFF02  jmp             -2                ; → PC 2533
  [ 2536]  10000005  yield           0x10            
  [ 2537]  10000005  yield           0x10            
  [ 2538]  01000015  push_cond       0x1             
  [ 2539]  7A010018  syscall         378               ; Make_operable
  [ 2540]  FF010018  syscall         511               ; Enter_event_mode
  [ 2541]  73000018  syscall         115               ; Command_display_off
  [ 2542]  71000018  syscall         113               ; Gauge_off
  [ 2543]  01000009  push            0x1             
  [ 2544]  08000018  syscall         8                 ; Set_wait_timer
  [ 2545]  07000009  push            0x7             
  [ 2546]  08000009  push            0x8             
  [ 2547]  02000009  push            0x2             
  [ 2548]  04000018  syscall         4                 ; Set_window_size
  [ 2549]  07000009  push            0x7             
  [ 2550]  06000009  push            0x6             
  [ 2551]  05000018  syscall         5                 ; Set_window_type
  [ 2552]  07000009  push            0x7             
  [ 2553]  00000009  push            0x0             
  [ 2554]  06000018  syscall         6                 ; Set_window_opening_speed
  [ 2555]  07000009  push            0x7             
  [ 2556]  00000009  push            0x0             
  [ 2557]  53000018  syscall         83                ; Set_window_close_speed
  [ 2558]  07000009  push            0x7             
  [ 2559]  00000009  push            0x0             
  [ 2560]  50000018  syscall         80                ; Set_window_tail_type
  [ 2561]  01000009  push            0x1             
  [ 2562]  08000018  syscall         8                 ; Set_wait_timer
  [ 2563]  07000009  push            0x7             
  [ 2564]  49000009  push            0x49              ; 73
  [ 2565]  DC000009  push            0xDC              ; 220
  [ 2566]  05000001  alu             and             
  [ 2567]  96000009  push            0x96              ; 150
  [ 2568]  05000001  alu             and             
  [ 2569]  6D010018  syscall         365               ; Set_window_width_auto
  [ 2570]  07000009  push            0x7             
  [ 2571]  00000018  syscall         0                 ; Open_window
  [ 2572]  07000009  push            0x7             
  [ 2573]  49000009  push            0x49              
  [ 2574]  01000018  syscall         1                 ; Display_message  0x49
  [ 2575]  07000009  push            0x7             
  [ 2576]  6B000018  syscall         107               ; Wait_message_end_ID
  [ 2577]  07000009  push            0x7             
  [ 2578]  02000018  syscall         2                 ; Close_window
  [ 2579]  00020018  syscall         512               ; Exit_event_mode
  [ 2580]  70000018  syscall         112               ; Gauge_on
  [ 2581]  72000018  syscall         114               ; Command_display_on
  [ 2582]  50020018  syscall         592               ; Remove_invincibility
  [ 2583]  01000015  push_cond       0x1             
  [ 2584]  79010018  syscall         377               ; Make_inoperable
  [ 2585]  10000005  yield           0x10        
```


## Traverse Town (Post-Final Boss) EVDL Files

The following `.evdl` files are loaded in **Traverse Town after defeating the final boss**.  
This is useful for identifying which scripts control each room in the endgame state.

| File | Location |
|------|---------|
| `tw01_ard5.evdl` | 1st District |
| `tw11_ard0.evdl` | Accessory Shop |
| `tw12_ard0.evdl` | Item Workshop |
| `tw10_ard2.evdl` | Item Shop |
| `tw13_ard0.evdl` | Geppetto's House |
| *(uses ARD EVDL)* | 2nd District |
| `tw08_ard19.evdl` | Hallway |
| `tw06_ard19.evdl` | Green Room |
| `tw07_ard19.evdl` | Red Room |
| `tw18_ard19.evdl` | Gizmo Shop |
| `tw17_ard0.evdl` | Dalmatian's House |
| `tw16_ard0.evdl` | Living Room |
| `tw15_ard0.evdl` | Dining Room |
| `tw14_ard0.evdl` | Dalmatian's Den |
| `tw05_ard19.evdl` | Alleyway |
| `tw23_ard0.evdl` | Secret Waterway |
| `tw20_ard0.evdl` | Magician's Study |
| `tw09_ard0.evdl` | Mystical House |
| `tw25_ard19.evdl` | 3rd District |
| `tw26_ard4.evdl` | Small House |

---

### Notes

- These scripts represent the **post-game world state**
- Depending on the game language it can be any of the languages but for english and international game uses the UK evdl files  
- Some areas reuse EVDL from their ARD instead of a unique file
