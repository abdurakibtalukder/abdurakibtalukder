<br>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/abdurakibtalukder/abdurakibtalukder/refs/heads/main/assets/Asset%206abdurakibtalukder-light.webp" width="70%">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/abdurakibtalukder/abdurakibtalukder/refs/heads/main/assets/Asset%207abdurakibtalukder-dark.webp" width="70%">
    <img alt="logo" src="https://raw.githubusercontent.com/abdurakibtalukder/abdurakibtalukder/refs/heads/main/assets/Asset%207abdurakibtalukder-dark.webp" width="70%">
  </picture>
</p>

<br>

```asm
; ═══════════════════════════════════════════════════
;  IDENTITY.ASM — abdurakibtalukder
; ═══════════════════════════════════════════════════

section .data
    name        db  "Abdul Rakib Talukder", 0
    age         db  15
    location    db  "Bangladesh", 0
    username    db  "@abdurakibtalukder", 0

section .education
    school      db  "Ambition Public School, Bhairab", 0
    degree      db  "Humanities — Arts & ICT", 0
    grad_year   dw  2026
    field       db  "Software Development", 0

section .career
    role        db  "Full Stack Developer", 0
    status      db  "BUSY", 0
    stack       db  "JavaScript", "React", "Node.js", "Python"
    stack_len   equ $ - stack

section .hobbies
    idx_0       db  "Open Source", 0
    idx_1       db  "Planning", 0
    idx_2       db  "Cycling", 0
    idx_3       db  "Gaming", 0

section .text
global _start

_start:
    MOV  AX,  [age]                     ; load current age
    CMP  AX,  18                        ; are we an adult yet?
    JL   .still_learning                ; nope — keep grinding

.still_learning:
    PUSH "Build clean, useful,"
    PUSH "and meaningful things."
    CALL philosophy
    JMP  _start                         ; loop forever — never stop
```
