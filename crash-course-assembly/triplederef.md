        Address │ Contents
      +────────────────────+
┌────▸│ 133700  │ 123400   │───┐
│     +────────────────────+   │
│ ┌──▸│ 123400  │ 100000   │─┐ │
│ │   +────────────────────+ │ │
│ │ ┌▸│ 100000  │ 42       │ │ │
│ │ │ +────────────────────+ │ │
│ │ └────────────────────────┘ │
│ └────────────────────────────┘
└──────────────────────────────┐
                               │
       Register │ Contents     │
      +────────────────────+   │
      │ rdi     │ 133700   │───┘
      +────────────────────+

As you can see, we'll place the first address that you must dereference into rdi. Go get the value!

mov rdi, [rdi]
mov rdi, [rdi]
mov rdi, [rdi]
mov rax, 60
syscall

