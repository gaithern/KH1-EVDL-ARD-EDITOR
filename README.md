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

Below is a real example of a BD script that continuously scales an object up and down:

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
