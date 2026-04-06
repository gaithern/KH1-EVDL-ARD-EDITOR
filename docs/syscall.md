# KH1 Syscall Reference

| Syscall Index (Dec) | Syscall Index (Hex) | Syscall Name |
|---------------------|---------------------|--------------|
| 0 | 0x0 | Open Window |
| 1 | 0x1 | Display Message |
| 2 | 0x2 | Close Window |
| 3 | 0x3 | Set Window Position |
| 4 | 0x4 | Set Window Size |
| 5 | 0x5 | Set Window Type |
| 6 | 0x6 | Set Window Opening Speed |
| 7 | 0x7 | Set Message Display Speed |
| 8 | 0x8 | Set Wait Timer |
| 9 | 0x9 | Display Register Value |
| 10 | 0xA | Set Char Id |
| 11 | 0xB | Move Char |
| 12 | 0xC | Rotate Char |
| 13 | 0xD | Change Motion |
| 14 | 0xE | Event Occurs |
| 15 | 0xF | Event Ends |
| 16 | 0x10 | Get Char Pos X |
| 17 | 0x11 | Get Char Pos Y |
| 18 | 0x12 | Get Char Pos Z |
| 19 | 0x13 | Set Char Position |
| 20 | 0x14 | Wait Move Done |
| 21 | 0x15 | Show Char |
| 22 | 0x16 | Hide Char |
| 23 | 0x17 | Show Char Shadow |
| 24 | 0x18 | Hide Char Shadow |
| 25 | 0x19 | Collision On |
| 26 | 0x1A | Collision Off |
| 27 | 0x1B | Fade In |
| 28 | 0x1C | Fade Out |
| 29 | 0x1D | White In |
| 30 | 0x1E | White Out |
| 31 | 0x1F | Blur On |
| 32 | 0x20 | Blur Off |
| 33 | 0x21 | Wait Message End |
| 34 | 0x22 | Play Camera Motion |
| 35 | 0x23 | Set Camera Position |
| 36 | 0x24 | Set Camera Focus Position |
| 37 | 0x25 | Rotate Camera |
| 38 | 0x26 | Set Camera Distance |
| 39 | 0x27 | Set Camera Fov |
| 40 | 0x28 | Get Camera Focus X |
| 41 | 0x29 | Get Camera Focus Y |
| 42 | 0x2A | Get Camera Focus Z |
| 43 | 0x2B | Get Camera Rot X |
| 44 | 0x2C | Get Camera Rot Y |
| 45 | 0x2D | Get Camera Rot Z |
| 46 | 0x2E | Get Camera Distance |
| 47 | 0x2F | Get Camera Fov |
| 48 | 0x30 | Start Effect |
| 49 | 0x31 | Move Camera Focus |
| 50 | 0x32 | Move Camera Rotation |
| 51 | 0x33 | Move Camera Distance |
| 52 | 0x34 | Move Camera Fov |
| 53 | 0x35 | Char Jump |
| 54 | 0x36 | Char Ctrl On |
| 55 | 0x37 | Char Ctrl Off |
| 56 | 0x38 | Motion Ctrl On |
| 57 | 0x39 | Motion Ctrl Off |
| 58 | 0x3A | Change Motion Interp |
| 59 | 0x3B | Change Map |
| 60 | 0x3C | Change Area |
| 61 | 0x3D | Get Event Starter Id |
| 62 | 0x3E | Group Display On |
| 63 | 0x3F | Group Display Off |
| 64 | 0x40 | Set Var 1 |
| 65 | 0x41 | Set Var 0 |
| 66 | 0x42 | Inc Var |
| 67 | 0x43 | Dec Var |
| 68 | 0x44 | Random Value |
| 69 | 0x45 | Turn Char |
| 70 | 0x46 | Turn Char Left |
| 71 | 0x47 | Turn Char Right |
| 72 | 0x48 | Add Light |
| 73 | 0x49 | Light Type |
| 74 | 0x4A | Light Position |
| 75 | 0x4B | Light Direction |
| 76 | 0x4C | Light Color |
| 77 | 0x4D | Point Light Distance |
| 78 | 0x4E | Spot Light Angle |
| 79 | 0x4F | Remove Light |
| 80 | 0x50 | Set Window Tail Type |
| 81 | 0x51 | Set Window Tail Location |
| 82 | 0x52 | Set Window Tail Rotation |
| 83 | 0x53 | Set Window Close Speed |
| 84 | 0x54 | Widescreen On |
| 85 | 0x55 | Widescreen Off |
| 86 | 0x56 | Change Motion Frame |
| 87 | 0x57 | Pause Motion |
| 88 | 0x58 | Enter Selection Mode |
| 89 | 0x59 | Wait Selection |
| 90 | 0x5A | Change Char Color |
| 91 | 0x5B | Restore Char Color |
| 92 | 0x5C | Load Event Motion |
| 93 | 0x5D | Wait File Load |
| 94 | 0x5E | Set Event Motion |
| 95 | 0x5F | Set Battle Motion |
| 96 | 0x60 | Hide Body Parts |
| 97 | 0x61 | Show Body Parts |
| 98 | 0x62 | Wait Turn End |
| 99 | 0x63 | Turn To Position |
| 100 | 0x64 | Save Crossfade Image |
| 101 | 0x65 | Start Crossfade |
| 102 | 0x66 | Camera Vibration |
| 103 | 0x67 | Wait Motion End |
| 104 | 0x68 | Char Bg On |
| 105 | 0x69 | Char Bg Off |
| 106 | 0x6A | Wait Event Camera End |
| 107 | 0x6B | Wait Message End Id |
| 108 | 0x6C | Motion Change No Loop |
| 109 | 0x6D | Start Texture Animation |
| 110 | 0x6E | Motion Change No Loop Interp |
| 111 | 0x6F | Motion Change No Loop Frame |
| 112 | 0x70 | Gauge On |
| 113 | 0x71 | Gauge Off |
| 114 | 0x72 | Command Display On |
| 115 | 0x73 | Command Display Off |
| 116 | 0x74 | Change Blur Alpha |
| 117 | 0x75 | Change Blur Color |
| 118 | 0x76 | Change Blur Width |
| 119 | 0x77 | Change Blur Height |
| 120 | 0x78 | Default Shadow Light On |
| 121 | 0x79 | Default Shadow Light Off |
| 122 | 0x7A | Change Char Scale |
| 123 | 0x7B | Play Partial Motion |
| 124 | 0x7C | Play Voice |
| 125 | 0x7D | Stop Voice |
| 126 | 0x7E | Trigger Event |
| 127 | 0x7F | Get World Number |
| 128 | 0x80 | Get Area Number |
| 129 | 0x81 | Get Set Number |
| 130 | 0x82 | Change Map Whiteout |
| 131 | 0x83 | Change Area Whiteout |
| 132 | 0x84 | Set Attribute On |
| 133 | 0x85 | Set Attribute Off |
| 134 | 0x86 | Write Set Number |
| 135 | 0x87 | Keyhole Fade Out |
| 136 | 0x88 | Event Sram Flag On |
| 137 | 0x89 | Event Sram Flag Off |
| 138 | 0x8A | Get Event Sram Flag |
| 139 | 0x8B | Widescreen On Quick |
| 140 | 0x8C | Widescreen Off Quick |
| 141 | 0x8D | Weapon Display On |
| 142 | 0x8E | Weapon Display Off |
| 143 | 0x8F | Stage Destruction Effect |
| 144 | 0x90 | Check Map Jump Press |
| 145 | 0x91 | Check Map Jump Motion |
| 146 | 0x92 | Check Map Landing |
| 147 | 0x93 | Play Camera Motion Local |
| 148 | 0x94 | Play Camera Motion Local Rot |
| 149 | 0x95 | Force Quit Script |
| 150 | 0x96 | All Char Ctrl On |
| 151 | 0x97 | All Char Ctrl Off |
| 152 | 0x98 | Check Char On Stage |
| 153 | 0x99 | Change Window Coords |
| 154 | 0x9A | Restore Camera |
| 155 | 0x9B | Add Bg Light |
| 156 | 0x9C | Restore Camera Default |
| 157 | 0x9D | Move Noturn |
| 158 | 0x9E | Set Valid Key Input |
| 159 | 0x9F | Clear Valid Key Input |
| 160 | 0xA0 | Switch To Battle Mode |
| 161 | 0xA1 | Switch To Normal Mode |
| 162 | 0xA2 | Clear Event Effect |
| 163 | 0xA3 | Start Resident Effect |
| 164 | 0xA4 | Clear Resident Effect |
| 165 | 0xA5 | Load Event Effect |
| 166 | 0xA6 | Wait Event Effect Load |
| 167 | 0xA7 | Change Resident Effect Coords |
| 168 | 0xA8 | Blur On2 |
| 169 | 0xA9 | Blur Off2 |
| 170 | 0xAA | Blur Type |
| 171 | 0xAB | Blur Distance |
| 172 | 0xAC | Get Pad Buttons |
| 173 | 0xAD | Get Pad Trigger |
| 174 | 0xAE | Play Camera Motion Local Rot 2actors |
| 175 | 0xAF | Face Actor |
| 176 | 0xB0 | Pauseflag Off |
| 177 | 0xB1 | Open Window No Close |
| 178 | 0xB2 | Activate Title Effect |
| 179 | 0xB3 | Start Talk Camera |
| 180 | 0xB4 | End Talk Camera |
| 181 | 0xB5 | Load Model |
| 182 | 0xB6 | Wait Model Load |
| 183 | 0xB7 | Display Model |
| 184 | 0xB8 | Rotate Blur |
| 185 | 0xB9 | Move Blur |
| 186 | 0xBA | Clear Loaded Effect Id |
| 187 | 0xBB | Clear Resident Effect Id |
| 188 | 0xBC | Set Loaded Effect Location |
| 189 | 0xBD | Set Loaded Effect Location Bone |
| 190 | 0xBE | Play Se |
| 191 | 0xBF | Stop Se |
| 192 | 0xC0 | Get Distance 2axis |
| 193 | 0xC1 | Get Distance 3axis |
| 194 | 0xC2 | Get Actor Distance 2axis |
| 195 | 0xC3 | Get Actor Distance 3axis |
| 196 | 0xC4 | Set Resident Effect Location Bone |
| 197 | 0xC5 | Get Current Command |
| 198 | 0xC6 | Set Command Speak Range |
| 199 | 0xC7 | Set Command Check Range |
| 200 | 0xC8 | Enable Menu Display |
| 201 | 0xC9 | Disable Menu Display |
| 202 | 0xCA | Get Angle Actor To Coord |
| 203 | 0xCB | Get Angle Between Actors |
| 204 | 0xCC | Fade Image In |
| 205 | 0xCD | Fade Image Out |
| 206 | 0xCE | Set Image Offset |
| 207 | 0xCF | Set Image Scale |
| 208 | 0xD0 | Set Camera Speed |
| 209 | 0xD1 | Set Motion Speed |
| 210 | 0xD2 | Set Effect Speed |
| 211 | 0xD3 | Set Object Far Clip |
| 212 | 0xD4 | Pause Actor |
| 213 | 0xD5 | Resume Actor |
| 214 | 0xD6 | Backload Test Event Motion |
| 215 | 0xD7 | Set Frame Color |
| 216 | 0xD8 | Start Frame Coloring |
| 217 | 0xD9 | Stop Frame Coloring |
| 218 | 0xDA | Turn Head Angle |
| 219 | 0xDB | Turn Head Coords |
| 220 | 0xDC | Turn Head Actor |
| 221 | 0xDD | Restore Head |
| 222 | 0xDE | Open Shop Buy |
| 223 | 0xDF | Wait Shop Close |
| 224 | 0xE0 | Move Jump |
| 225 | 0xE1 | Display Record |
| 226 | 0xE2 | Hide Record |
| 227 | 0xE3 | Show Timer |
| 228 | 0xE4 | Hide Timer |
| 229 | 0xE5 | Start Timer Up |
| 230 | 0xE6 | Start Timer Down |
| 231 | 0xE7 | Pause Timer |
| 232 | 0xE8 | Restart Timer |
| 233 | 0xE9 | Stop Timer |
| 234 | 0xEA | Set Max Counter |
| 235 | 0xEB | Inc Counter |
| 236 | 0xEC | Show Counter |
| 237 | 0xED | Hide Counter |
| 238 | 0xEE | Start Minigame |
| 239 | 0xEF | End Minigame |
| 240 | 0xF0 | Show Ranking |
| 241 | 0xF1 | Start Hercules Event |
| 242 | 0xF2 | Reset Timer |
| 243 | 0xF3 | Message To Battle Script |
| 244 | 0xF4 | Load Image |
| 245 | 0xF5 | Wait Image Load |
| 246 | 0xF6 | Display Image |
| 247 | 0xF7 | Hide Image |
| 248 | 0xF8 | Scroll Image Y |
| 249 | 0xF9 | Load Bgm |
| 250 | 0xFA | Wait Bgm Load |
| 251 | 0xFB | Play Bgm |
| 252 | 0xFC | Restore Bgm |
| 253 | 0xFD | Check Bag Item Count |
| 254 | 0xFE | Set Loaded Effect Start Frame |
| 255 | 0xFF | Set Resident Effect Start Frame |
| 256 | 0x100 | Load Voice |
| 257 | 0x101 | Wait Voice Load |
| 258 | 0x102 | Change Bag Items |
| 259 | 0x103 | Check Char In Area |
| 260 | 0x104 | Start Vibration |
| 261 | 0x105 | Stop Vibration |
| 262 | 0x106 | Clipping On |
| 263 | 0x107 | Clipping Off |
| 264 | 0x108 | Set Motion Null To Char Pos |
| 265 | 0x109 | Set Char Run Speed |
| 266 | 0x10A | Reset Char Run Speed |
| 267 | 0x10B | Change Char Weight |
| 268 | 0x10C | Open Shop Sell |
| 269 | 0x10D | Add Party Member |
| 270 | 0x10E | Remove Party Member |
| 271 | 0x10F | Get Motion Null X |
| 272 | 0x110 | Get Motion Null Y |
| 273 | 0x111 | Get Motion Null Z |
| 274 | 0x112 | Go To World Map |
| 275 | 0x113 | Hercules Win Menu |
| 276 | 0x114 | Hercules Lose Menu |
| 277 | 0x115 | Hercules Champion Menu |
| 278 | 0x116 | Game Over |
| 279 | 0x117 | Quick Save |
| 280 | 0x118 | Move Slow |
| 281 | 0x119 | Get Part From Party |
| 282 | 0x11A | Display Black Image |
| 283 | 0x11B | Display New Record |
| 284 | 0x11C | Push Actor Coord X |
| 285 | 0x11D | Push Actor Coord Y |
| 286 | 0x11E | Push Actor Coord Z |
| 287 | 0x11F | Push Actor Rotation |
| 288 | 0x120 | Push Runlevel |
| 289 | 0x121 | Push Motion Frames |
| 290 | 0x122 | Push Actor Coord X2 |
| 291 | 0x123 | Push Actor Coord Y2 |
| 292 | 0x124 | Push Actor Coord Z2 |
| 293 | 0x125 | Push Actor Rotation2 |
| 294 | 0x126 | Push Runlevel2 |
| 295 | 0x127 | Push Motion Frames2 |
| 296 | 0x128 | Fade In Image Black Bg |
| 297 | 0x129 | Fade Out Image Black Bg |
| 298 | 0x12A | Cancel Movement |
| 299 | 0x12B | Move To Actor Pos |
| 300 | 0x12C | Enable Game Over |
| 301 | 0x12D | Disable Game Over |
| 302 | 0x12E | Keyhole Fade In |
| 303 | 0x12F | End Keyhole Fade |
| 304 | 0x130 | Set Sky Initial Rotation |
| 305 | 0x131 | Get Minigame Menu Selection |
| 306 | 0x132 | Set Char Initial State |
| 307 | 0x133 | Call Sin |
| 308 | 0x134 | Call Cos |
| 309 | 0x135 | Check Char In Camera |
| 310 | 0x136 | Check Battle Or Normal Mode |
| 311 | 0x137 | Get Camera Viewpoint X |
| 312 | 0x138 | Get Camera Viewpoint Y |
| 313 | 0x139 | Get Camera Viewpoint Z |
| 314 | 0x13A | Get Attack Type Id |
| 315 | 0x13B | Erase All Map Objects |
| 316 | 0x13C | Show All Map Objects |
| 317 | 0x13D | Fade In 3d |
| 318 | 0x13E | Fade Out 3d |
| 319 | 0x13F | Discard Object Data |
| 320 | 0x140 | Enable Targeting |
| 321 | 0x141 | Disable Targeting |
| 322 | 0x142 | Get Motion Number |
| 323 | 0x143 | Add Hp |
| 324 | 0x144 | Add Mp |
| 325 | 0x145 | Wait All Enemies Defeated |
| 326 | 0x146 | Enable Magic Command |
| 327 | 0x147 | Disable Magic Command |
| 328 | 0x148 | Enable Item Command |
| 329 | 0x149 | Disable Item Command |
| 330 | 0x14A | Enable Summon Command |
| 331 | 0x14B | Disable Summon Command |
| 332 | 0x14C | Set Counter Value |
| 333 | 0x14D | Get Holdable Count |
| 334 | 0x14E | Check First Person View |
| 335 | 0x14F | Make Not Invincible |
| 336 | 0x150 | Make Invincible |
| 337 | 0x151 | Make Pressable |
| 338 | 0x152 | Make Non Pressable |
| 339 | 0x153 | Set Treasure Flag |
| 340 | 0x154 | Get Treasure Flag |
| 341 | 0x155 | Get Treasure Number |
| 342 | 0x156 | Get Treasure Type |
| 343 | 0x157 | Get Treasure Value |
| 344 | 0x158 | Erase Treasure |
| 345 | 0x159 | Get Treasure Id |
| 346 | 0x15A | Enemy Ctrl On |
| 347 | 0x15B | Enemy Ctrl Off |
| 348 | 0x15C | Activate Battle Effects |
| 349 | 0x15D | Set Battle Effect To Bone |
| 350 | 0x15E | Set Party |
| 351 | 0x15F | Move Smooth Rot |
| 352 | 0x160 | Change Game Speed |
| 353 | 0x161 | Play Se2 |
| 354 | 0x162 | Set Little Mermaid Water Speed |
| 355 | 0x163 | Get Comm Id |
| 356 | 0x164 | Get Comm Num |
| 357 | 0x165 | Set Comm Work |
| 358 | 0x166 | Display Item Acquired Message |
| 359 | 0x167 | Display Money Acquired Message |
| 360 | 0x168 | Disable Battle Event Box |
| 361 | 0x169 | Enable Battle Event Box |
| 362 | 0x16A | Disable All Battle Event Boxes |
| 363 | 0x16B | Enable All Battle Event Boxes |
| 364 | 0x16C | Set Item Number In Message |
| 365 | 0x16D | Set Window Width Auto |
| 366 | 0x16E | Get Party Count |
| 367 | 0x16F | Display Prize |
| 368 | 0x170 | Hide Prize |
| 369 | 0x171 | Delete Prize |
| 370 | 0x172 | Return To Title |
| 371 | 0x173 | Change Effect Rotation |
| 372 | 0x174 | Change Effect Scale |
| 373 | 0x175 | Change Resident Effect Rotation |
| 374 | 0x176 | Change Resident Effect Scale |
| 375 | 0x177 | Make Not Invincible Actor |
| 376 | 0x178 | Make Invincible Actor |
| 377 | 0x179 | Make Inoperable |
| 378 | 0x17A | Make Operable |
| 379 | 0x17B | Get Char Current Area |
| 380 | 0x17C | End Effect Loop |
| 381 | 0x17D | End Resident Effect Loop |
| 382 | 0x17E | Add Event Box |
| 383 | 0x17F | Count Objects By Part |
| 384 | 0x180 | Load Event Se |
| 385 | 0x181 | Wait Event Se Load |
| 386 | 0x182 | Delete Event Box |
| 387 | 0x183 | Get Char Hp |
| 388 | 0x184 | Get Char Mp |
| 389 | 0x185 | Write Set Number From Table |
| 390 | 0x186 | Start Bgse |
| 391 | 0x187 | Stop Bgse |
| 392 | 0x188 | Call Name Input |
| 393 | 0x189 | Get Char Weight |
| 394 | 0x18A | Hold Camera Info |
| 395 | 0x18B | Get Camera Info |
| 396 | 0x18C | Fisheye On |
| 397 | 0x18D | Fisheye Off |
| 398 | 0x18E | Map Display On |
| 399 | 0x18F | Map Display Off |
| 400 | 0x190 | Set Camera Parameters |
| 401 | 0x191 | Reset Camera Parameters |
| 402 | 0x192 | Stealth On |
| 403 | 0x193 | Stealth Off |
| 404 | 0x194 | Get Motion Number Actor |
| 405 | 0x195 | Load Waveform |
| 406 | 0x196 | Wait Waveform Load |
| 407 | 0x197 | Party Gauge On |
| 408 | 0x198 | Party Gauge Off |
| 409 | 0x199 | Restore Se |
| 410 | 0x19A | Wait Restore Music |
| 411 | 0x19B | Get Ground Color From Area |
| 412 | 0x19C | Set Ground Color To Polygon |
| 413 | 0x19D | Quick Save On |
| 414 | 0x19E | Quick Save Off |
| 415 | 0x19F | Stop Bgm |
| 416 | 0x1A0 | Add Battle Item |
| 417 | 0x1A1 | Pad Ctrl On |
| 418 | 0x1A2 | Pad Ctrl Off |
| 419 | 0x1A3 | Getlength 2 |
| 420 | 0x1A4 | Getlength3 2 |
| 421 | 0x1A5 | Getlengtha 2 |
| 422 | 0x1A6 | Getlength3a 2 |
| 423 | 0x1A7 | Char Request On |
| 424 | 0x1A8 | Char Request Off |
| 425 | 0x1A9 | Stop Se All |
| 426 | 0x1AA | Erase All Enemies |
| 427 | 0x1AB | Change Bgm Volume |
| 428 | 0x1AC | Add Mp Charge |
| 429 | 0x1AD | Mp Charge On |
| 430 | 0x1AE | Mp Charge Off |
| 431 | 0x1AF | Motion Sound On |
| 432 | 0x1B0 | Motion Sound Off |
| 433 | 0x1B1 | Ground Sound On |
| 434 | 0x1B2 | Ground Sound Off |
| 435 | 0x1B3 | Play Effect Sound |
| 436 | 0x1B4 | Stop Effect Sound |
| 437 | 0x1B5 | Show Object From Callnum |
| 438 | 0x1B6 | Check Sora On Ground |
| 439 | 0x1B7 | Get Enemies Killed |
| 440 | 0x1B8 | Reset Enemies Killed |
| 441 | 0x1B9 | Disable Battle Mode Entry |
| 442 | 0x1BA | Enable Battle Mode Entry |
| 443 | 0x1BB | Wait Voice Finish |
| 444 | 0x1BC | Increase Money |
| 445 | 0x1BD | Load Next Map Texture |
| 446 | 0x1BE | Set Effect Rotation From Bone |
| 447 | 0x1BF | Set Effect Rotation From Bone2 |
| 448 | 0x1C0 | Enemy View Off |
| 449 | 0x1C1 | Enemy View On |
| 450 | 0x1C2 | Load All Objects Callnum |
| 451 | 0x1C3 | Wait All Objects Callnum |
| 452 | 0x1C4 | Get Mapobj Bg Color |
| 453 | 0x1C5 | Get Distance To Nearest Enemy |
| 454 | 0x1C6 | Set Special Command |
| 455 | 0x1C7 | Get Special Command Count |
| 456 | 0x1C8 | Display Defeated Enemy Count |
| 457 | 0x1C9 | Get Enemies In Zone |
| 458 | 0x1CA | Load Magic |
| 459 | 0x1CB | Wait Magic Load |
| 460 | 0x1CC | Get Magic Level |
| 461 | 0x1CD | Load All Objects Zone |
| 462 | 0x1CE | Wait Zone Load |
| 463 | 0x1CF | Set Special Thread Return |
| 464 | 0x1D0 | Move Jump Frame |
| 465 | 0x1D1 | Change Hercules Ranking |
| 466 | 0x1D2 | Enable Accel Zone |
| 467 | 0x1D3 | Disable Accel Zone |
| 468 | 0x1D4 | Slider Ctrl On |
| 469 | 0x1D5 | Slider Ctrl Off |
| 470 | 0x1D6 | Init Battle Script |
| 471 | 0x1D7 | Init All Enemy Battle Scripts |
| 472 | 0x1D8 | Get Attack Type Received |
| 473 | 0x1D9 | Get Map Object Damage |
| 474 | 0x1DA | Get Battle Count |
| 475 | 0x1DB | Set Message Numerical Work |
| 476 | 0x1DC | Enable Event Skipping |
| 477 | 0x1DD | Disable Event Skipping |
| 478 | 0x1DE | Release Object Callnum |
| 479 | 0x1DF | Set Growth Type 1 |
| 480 | 0x1E0 | Set Growth Type 2 |
| 481 | 0x1E1 | Change Sora Parameters |
| 482 | 0x1E2 | Set Magic Minus Flag |
| 483 | 0x1E3 | Set Item Minus Flag |
| 484 | 0x1E4 | Set Special Minus Flag |
| 485 | 0x1E5 | Change Weapon |
| 486 | 0x1E6 | Force Event Pose |
| 487 | 0x1E7 | Force No Event Pose |
| 488 | 0x1E8 | Open Gummy Menu |
| 489 | 0x1E9 | Start Movie |
| 490 | 0x1EA | Wait Movie End |
| 491 | 0x1EB | Write Other World Set Number |
| 492 | 0x1EC | Clear History |
| 493 | 0x1ED | Set Save Point Flag |
| 494 | 0x1EE | Get Save Point Flag |
| 495 | 0x1EF | Delete Save Point |
| 496 | 0x1F0 | Start Map Change |
| 497 | 0x1F1 | Wait Name Input |
| 498 | 0x1F2 | Add Party Menu Command |
| 499 | 0x1F3 | Set Polygon Attribute |
| 500 | 0x1F4 | Set Polygon Kind |
| 501 | 0x1F5 | Set Polygon Ground |
| 502 | 0x1F6 | Get Time Since Start |
| 503 | 0x1F7 | Learn Magic |
| 504 | 0x1F8 | Change Song Bank |
| 505 | 0x1F9 | Wait Music Jump |
| 506 | 0x1FA | Change Track Volume |
| 507 | 0x1FB | Sky2 Display On |
| 508 | 0x1FC | Sky2 Display Off |
| 509 | 0x1FD | Change Fog |
| 510 | 0x1FE | Set Fog Default |
| 511 | 0x1FF | Enter Event Mode |
| 512 | 0x200 | Exit Event Mode |
| 513 | 0x201 | Event Camera On |
| 514 | 0x202 | Event Camera Off |
| 515 | 0x203 | Move Noturn |
| 516 | 0x204 | Rot |
| 517 | 0x205 | Check Map Changeable |
| 518 | 0x206 | Add Char To Dictionary |
| 519 | 0x207 | Check Char In Dictionary |
| 520 | 0x208 | Add Dalmatian |
| 521 | 0x209 | Check Dalmatian |
| 522 | 0x20A | Update Minigame Record |
| 523 | 0x20B | Get Minigame Record |
| 524 | 0x20C | Set Story Flag |
| 525 | 0x20D | Get Story Flag |
| 526 | 0x20E | Add Anthem Report |
| 527 | 0x20F | Check Anthem Report |
| 528 | 0x210 | Open Party Menu |
| 529 | 0x211 | Remove Char From Dictionary |
| 530 | 0x212 | Remove Story Flag |
| 531 | 0x213 | Update Minigame Record 100kills |
| 532 | 0x214 | Change Camera Sora Distance |
| 533 | 0x215 | Get Camera Sora Distance |
| 534 | 0x216 | Set Battle Message Return |
| 535 | 0x217 | Play Obj Effect |
| 536 | 0x218 | Change Obj Effect Scale |
| 537 | 0x219 | Change Obj Effect Coords |
| 538 | 0x21A | Erase Obj Effect |
| 539 | 0x21B | Underwater Camera On |
| 540 | 0x21C | Underwater Camera Off |
| 541 | 0x21D | Get Char Action |
| 542 | 0x21E | Fade Out Map Group |
| 543 | 0x21F | Fade In Map Group |
| 544 | 0x220 | Load World Map Char |
| 545 | 0x221 | Wait World Map Char Load |
| 546 | 0x222 | Open World Map Window |
| 547 | 0x223 | Close World Map Window |
| 548 | 0x224 | Set World Map Char |
| 549 | 0x225 | Set World Map Char Motion |
| 550 | 0x226 | Set World Map Char Texture Animation |
| 551 | 0x227 | Display World Map Message |
| 552 | 0x228 | Scatter Map Gimmick Prizes |
| 553 | 0x229 | Check Coconuts Erasable |
| 554 | 0x22A | Feel Icon On |
| 555 | 0x22B | Feel Icon Off |
| 556 | 0x22C | Acquire Ability |
| 557 | 0x22D | Set Gummy Name Message |
| 558 | 0x22E | Set Ability Name Message |
| 559 | 0x22F | Set Magic Name Message |
| 560 | 0x230 | Set Summon Name Message |
| 561 | 0x231 | Enable Limit Technique |
| 562 | 0x232 | Disable Limit Technique |
| 563 | 0x233 | Load Bgm Motion Bank2 |
| 564 | 0x234 | Load Wave Motion Bank2 |
| 565 | 0x235 | Learn Summon |
| 566 | 0x236 | Summon End Command |
| 567 | 0x237 | Add Gummy |
| 568 | 0x238 | Restore Hp Mp |
| 569 | 0x239 | Wait Limit Skill End |
| 570 | 0x23A | Wait Summon End |
| 571 | 0x23B | Wait Se Finish |
| 572 | 0x23C | Wait Battle Icon Display |
| 573 | 0x23D | Wait Restore Se |
| 574 | 0x23E | Transfer Object Se |
| 575 | 0x23F | Wait Object Se Transfer |
| 576 | 0x240 | Clear Object Se |
| 577 | 0x241 | Check Save Menu Opened |
| 578 | 0x242 | Get Item From Gift Table |
| 579 | 0x243 | Movie Standby |
| 580 | 0x244 | Wait Movie Standby |
| 581 | 0x245 | Set Game Clear Flag |
| 582 | 0x246 | Get Game Clear Flag |
| 583 | 0x247 | Display Gauge Fadein |
| 584 | 0x248 | Remove Gauge Fadeout |
| 585 | 0x249 | Display Command Fadein |
| 586 | 0x24A | Remove Command Fadeout |
| 587 | 0x24B | Remove Invincibility |
| 588 | 0x24C | Make Party Invincible |
| 589 | 0x24D | Set World Map Flag |
| 590 | 0x24E | Get World Map Flag |
| 591 | 0x24F | Read Set Number |
| 592 | 0x250 | Start Map Effect |
| 593 | 0x251 | Change Map Effect Pos |
| 594 | 0x252 | Change Map Effect Rot |
| 595 | 0x253 | Change Map Effect Scale |
| 596 | 0x254 | Wait Name Input |
| 597 | 0x255 | Add Party Menu Command |
| 598 | 0x256 | Set Polygon Attribute |
| 599 | 0x257 | Set Polygon Kind |
| 600 | 0x258 | Change Map Effect Scale |
| 601 | 0x259 | Clear Map Effect
| 602 | 0x25A | Change Map Effect Start Frame
| 603 | 0x25B | End Map Effect Loop
| 604 | 0x25C | Bind Map Effect To Bone
| 605 | 0x25D | Display Message From Gift Table
| 606 | 0x25E | Change Char Color From Map Table
| 607 | 0x25F | Load All Enemy SE
| 608 | 0x260 | Play Object Effect Once
| 609 | 0x261 | Start Weapon Effect
| 610 | 0x262 | Clear Weapon Effect
| 611 | 0x263 | Change Permanent Effect Color
| 612 | 0x264 | Start Map Change Rewrite Set
| 613 | 0x265 | Get Char Level
| 614 | 0x266 | Get BG Color R
| 615 | 0x267 | Get BG Color G
| 616 | 0x268 | Get BG Color B
| 617 | 0x269 | Set Object BG Color
| 618 | 0x26A | Extract Set BG Color
| 619 | 0x26B | Bind Effect To Null
| 620 | 0x26C | Erase Weak Enemies
| 621 | 0x26D | Enable Blur No Update
| 622 | 0x26E | Check Object Touching Zone
| 623 | 0x26F | Widescreen On Frame
| 624 | 0x270 | Widescreen Off Frame
| 625 | 0x271 | Set Special Command Range
| 626 | 0x272 | Change Appear Flag
| 627 | 0x274 | Gummy Shop Buy
| 628 | 0x275 | Gummy Shop Sell
| 629 | 0x279 | Set Hercules Victory Flag
| 630 | 0x27A | Get Hercules Victory Flag
| 631 | 0x27B | Set Magic Name Message Multi
| 632 | 0x27C | Change Char Action
| 633 | 0x27D | Play Effect Bound Bone 2
| 634 | 0x27E | Get Dalmatians Collected
| 635 | 0x27F | Show Feel Icon
| 636 | 0x280 | Hide Feel Icon
| 637 | 0x281 | Speed Fix Move No Turn
| 638 | 0x282 | Load BGM On Map Change
| 639 | 0x283 | No BGM Load On Map Change
| 640 | 0x284 | Get Item Type
| 641 | 0x285 | Get Owned Money
| 642 | 0x286 | Wait Hercules Ranking Close
| 643 | 0x287 | Play Battle Voice
| 644 | 0x288 | Enable Gummies In Item Menu
| 645 | 0x289 | Get Counter Value
| 646 | 0x28A | Get Timer Value
| 647 | 0x28B | Restore Music Fadein
| 648 | 0x28C | Play Music Fadein
| 649 | 0x28E | Apply Effect To Bone Pos
| 650 | 0x28F | Rotate Effect To Bone Angle
| 651 | 0x290 | Worldmap Test
| 652 | 0x291 | Load Weapon
| 653 | 0x292 | Wait Weapon Load
| 654 | 0x293 | Fade Out SE
| 655 | 0x294 | Show Minigame Info
| 656 | 0x295 | Hide Minigame Info
| 657 | 0x296 | End DH Stage Destruction
| 658 | 0x2A1 | Synthesis Shop Menu Open
| 659 | 0x2A6 | Minigame Limit On
| 660 | 0x2A7 | Minigame Limit Off
| 661 | 0x2A8 | Cancel Ignore Sound
| 662 | 0x2A9 | Set Jiminy Memo Flag
| 663 | 0x2AA | Get Jiminy Memo Flag
| 664 | 0x2AB | Equip Weapon
| 665 | 0x2AC | Equip Accessory
| 666 | 0x2AD | Equip Ability
| 667 | 0x2B1 | Get Enemies Killed 2
| 668 | 0x2B2 | Get Enemies Killed All
| 669 | 0x2B4 | Get Hercules Team
| 670 | 0x2B5 | Get Hercules Ranking
| 671 | 0x2B7 | Scale Window From Gift
| 672 | 0x2B8 | Push Actor HP
| 673 | 0x2B9 | Push Actor MP
| 674 | 0x2BA | Play Effect Bound Bone 3
| 675 | 0x2BB | Play Effect Bound Bone 4
| 676 | 0x2BC | Enable Flight
| 677 | 0x2BD | Disable Flight
| 678 | 0x2BE | Enable Polygon Touch Event
| 679 | 0x2BF | Disable Polygon Touch Event
| 680 | 0x2C0 | Get Mapobj BG Color Frames
| 681 | 0x2C1 | Extract Set BG Color Frames
| 682 | 0x2C2 | Apply Effect To Bone Pos 2
| 683 | 0x2C3 | Rotate Effect To Bone Angle 2
| 684 | 0x2C4 | Wait Button Press
| 685 | 0x2C5 | Gummi Ship Event Message
| 686 | 0x2C6 | Stop All Enemy Scripts
| 687 | 0x2C7 | Run All Enemy Scripts
| 688 | 0x2C8 | Gummi Ship Tutorial
| 689 | 0x2C9 | Get Sora Gameover Motion
| 690 | 0x2CA | Load System Music
| 691 | 0x2CB | Wait System Music Load
| 692 | 0x2CC | Load Nightmare Effects
| 693 | 0x2CD | Wait Nightmare Effects Load
| 694 | 0x2CE | Get Equipped Weapon
| 695 | 0x2CF | Disable Battle Field Music Switch
| 696 | 0x2D0 | Enable Battle Field Music Switch
| 697 | 0x2D1 | Beevsetstickval
| 698 | 0x2D2 | Check Weapon Displayed
| 699 | 0x2D3 | Slow Wait
| 700 | 0x2D4 | Load System Music 2
| 701 | 0x2D5 | Restore BGM 2
| 702 | 0x2D6 | Restore Music Fadein 2
| 703 | 0x2D7 | Set Shadow Steal Flag
| 704 | 0x2D8 | Get Synthesiser Progress
| 705 | 0x2D9 | Set BG Color To Drawing
| 706 | 0x2DA | Stop SE 3D
| 707 | 0x2DB | Color Change No Invalidate Floor
| 708 | 0x2DC | Disable Ability
| 709 | 0x2DD | Unlock Ability Disable
| 710 | 0x2DE | Load Map Team Effect
| 711 | 0x2DF | Fill Gummy Parts
| 712 | 0x2E0 | Beevcheckwait
| 713 | 0x2E1 | Get Pad Buttons 2
| 714 | 0x2E2 | Show Party Weapons
| 715 | 0x2E3 | Hide Party Weapons
| 716 | 0x2E4 | Change Raft Name Highwind
| 717 | 0x2E5 | Message Full Gummy Set
| 718 | 0x2E6 | Get Player Continues Entering Map
| 719 | 0x2E7 | Set Minigame Played Flag
| 720 | 0x2E8 | Check Shared Ability Taken
| 721 | 0x2E9 | Wmevcheckobjmotion
| 722 | 0x2EA | Get Treasure Chest Full Flag
| 723 | 0x2EB | Check Bag Item Count Only
| 724 | 0x2EC | Enemy BG Impact On
| 725 | 0x2ED | Enemy BG Impact Off
| 726 | 0x2EE | Wmevstartwintexanime 2
| 727 | 0x2EF | Show Battle Counter Ending
| 728 | 0x2F0 | Check Bag Item Count 2
| 729 | 0x2F1 | Get Window X
| 730 | 0x2F2 | Get Window Y
| 731 | 0x2F3 | Check Expert Mode
| 732 | 0x2F4 | White In 3D
| 733 | 0x2F5 | White Out 3D
| 734 | 0x2F6 | Check Easy Mode
| 735 | 0x2F7 | Set Event Skip Flag
| 736 | 0x2F8 | Get Event Skip Flag
| 737 | 0x2F9 | Open Event Skip Menu
| 738 | 0x2FA | Get Event Skip Menu Selection
| 739 | 0x2FB | Get Jiminy Memo Complete