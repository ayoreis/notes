# Vim

Numbers work for almost all commands, like `3 }` for 3 code blocks up.

- `k` Up and `<n> k` for `n` lines
- `j` Down and `<n> j` for `n` lines
- `l` Right and `<n> l` for `n` lines
- `h` Left and `<n> h` for `n` lines
- `gg` Beginning of file
- `G` End of file
- `}` Up a block (lines until blank line)
- `{` Down a block
- `b` Previous word/punctuation
- `B` Previous after space
- `w` Next word/punctuation
- `W` Next after space
- `0` Start of line
- `^` First non-whitespace of line
- `$` End of line
- `t <x>` Go to before next `x` in line
- `f <x>` Go to next `x` in line
- `%` Pair brace/bracket (`d %`!)
- `*` Find next same word
- `;` Move to next same character
- `<n>G` Go to line number `n`
- `H` (Home) first visible line
- `M` Middle visible line
- `L` Last visible line
- `z` Centere viewport on line

- `i` Enter insert mode before cursor
- `a` Enter insert mode after cursor
- `I` Enter insert mode at the beginning of line
- `A` Enter insert mode at the end of line
- `o` Insert line below
- `O` Insert line above
- `esc` Exit insert mode

- `:` Command more
- `<n>` Go to line `n`

- `Ctrl v` Select in rectangle
- `r<x>` Replace with to `x` (`3r7!)
- `R<x+>` Replace `x.length` characters with `x`
- `~` Swap/switch case
- `x` Delete character
- `dd` Delete line
- `d <move command>` Delete until where it would move to, `esc` to cancel (`d t }`!)
- `D` Delete rest of line
- `c <move command>` Change
- `C` Change rest of line
- `u` Undo
- `Ctrl R` Redo
- `.` Repeat last command
- `yy` Copy line
- `p` Paste below cursor
- `P` Paste above cursor
- `v` Visual mode, all the movement command are available, when you other commands they will execute and return you to normal mode
- `V` Visual line mode
