# KH1 EV Op Code Reference

| EV Op Code Index (Dec) | EV Op Code Index (Hex) | Syscall Name |
|---------------------|---------------------|--------------|
| 0 | 0x0 | NOP |
| 1 | 0x1 | ALU |
| 2 | 0x2 | JMP |
| 3 | 0x3 | BEQZ |
| 4 | 0x4 | NOP |
| 5 | 0x5 | YIELD |
| 6 | 0x6 | STORE_REG |
| 7 | 0x7 | CMP_REG_IMM |
| 8 | 0x8 | DEC_REG_IDX |
| 9 | 0x9 | PUSH |
| 10 | 0xA | LOAD_LOCAL |
| 11 | 0xB | STORE_LOCAL |
| 12 | 0xC | READ_BYTE |
| 13 | 0xD | WRITE_BYTE |
| 14 | 0xE | READ_WORD |
| 15 | 0xF | WRITE_WORD |
| 16 | 0x10 | READ_DWORD |
| 17 | 0x11 | WRITE_DWORD |
| 18 | 0x12 | NOP |
| 19 | 0x13 | NOP |
| 20 | 0x14 | NOP |
| 21 | 0x15 | PUSH_COND |
| 22 | 0x16 | INIT_CALL |
| 23 | 0x17 | AWAIT_CALL |
| 24 | 0x18 | SYSCALL |
| 25 | 0x19 | FLOW_CTRL |
| 26 | 0x1A | SET_LT |
| 27 | 0x1B | SET_LE |
| 28 | 0x1C | SET_GT |
| 29 | 0x1D | SET_GE |
| 30 | 0x1E | READ_BIT |
| 31 | 0x1F | WRITE_BIT |