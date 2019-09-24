[//]: # (vim) Cheatsheet for vim
Quick tips:

- Mark a position as {a-z}: `m {a-z}`
- Move to a position {a-z}: `' {a-z}`
- Move to previous position: `"`
- Convert vi/vim tabs to spaces: `:1,$s/\t/ /g`
    - Remove the `g` to only do the first tab on each line
- Open last edited file: `CTRL+o+o`
- Output shell command (`ls` in this case): `:r !ls`
- Write to file when you forgot to sudo: `:w !sudo tee %`
- Scoll screen to make current line (of window)
    - `zz` the middle
    - `zt` the top
    - `zb` the bottom
- Go to older/new positions (from jumping around): `^O` or `^I`
- Go to last Insert mode position: `gi`
- Open file under cursor: `gf`
- Open file:linenumber under cursor: `gF`

Delete Tricks:

- Delete the current word: `diw`
- Delete within the current parentheses: `di(`
- Delete within the quotes: `di"`

How to use vim Macros (quick start):

- Create a recording on register **d**: `qd`
- During recording just perform your commands like normal
- Stop recording: `q`
- Execute Macro from register **d**: `@d`
- Execute the last macro executed: `@@`

How to use vim registers (quick start):

In normal mode:

- To yank into register `d`: `"dy`
- To paste from register `d`: `"dp`
- Yanking without a register goes to the `0` register
- The default register is the `"` register
- The `0` register is populated with **only** yanks
- The `"` register is also populated with `d/D/x/X/c/C/s/S`
- Use `:reg` to view the values in the registers
