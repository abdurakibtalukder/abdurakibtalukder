; ============================================
; README.md
; ============================================
; Author: Abdur Rakib Talukder
; Motto : No means next opportunity — keep moving.
; ============================================

section .data
    name        db "Rakib", 0
    role        db "Student | Learner | Developer", 0
    passion     db "I like tough code.", 0
    mindset     db "No means next opportunity.", 0

section .text
    global _start

_start:

    ; Initialize mindset
    mov eax, LEARN
    call practice_daily

    ; Solve problems
    mov ebx, CHALLENGES
    call solve

    ; Debug life
    call debug
    jmp improve

practice_daily:
    ; Keep coding
    inc skill_level
    ret

solve:
    ; Break problem
    ; Think
    ; Build solution
    ret

debug:
    ; Find errors
    ; Fix errors
    ; Repeat
    ret

improve:
    ; Infinite growth loop
    jmp practice_daily

; ============================================
; End of File
; Keep Moving Forward.
; ============================================
