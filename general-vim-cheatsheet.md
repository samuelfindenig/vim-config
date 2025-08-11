# Vim General Cheatsheet

## Modes

- `i` - Insert mode (before cursor)
- `a` - Insert mode (after cursor)
- `A` - Insert mode (end of line)
- `o` - Insert mode (new line below)
- `O` - Insert mode (new line above)
- `Esc` - Normal mode
- `v` - Visual mode (character selection)
- `V` - Visual line mode
- `Ctrl+v` - Visual block mode
- `:` - Command mode

## Basic Movement

- `h` - Left
- `j` - Down
- `k` - Up
- `l` - Right
- `w` - Next word
- `b` - Previous word
- `e` - End of current word
- `0` - Beginning of line
- `^` - First non-blank character of line
- `$` - End of line
- `gg` - Go to first line
- `G` - Go to last line
- `{number}G` - Go to line number
- `Ctrl+f` - Page down
- `Ctrl+b` - Page up
- `Ctrl+d` - Half page down
- `Ctrl+u` - Half page up

## Editing Commands

### Delete
- `x` - Delete character under cursor
- `X` - Delete character before cursor
- `dw` - Delete word
- `dd` - Delete line
- `d$` - Delete to end of line
- `d0` - Delete to beginning of line
- `D` - Delete to end of line (same as d$)

### Copy (Yank)
- `yy` - Copy line
- `yw` - Copy word
- `y$` - Copy to end of line
- `y0` - Copy to beginning of line

### Paste
- `p` - Paste after cursor/below line
- `P` - Paste before cursor/above line

### Change
- `cw` - Change word
- `cc` - Change line
- `c$` - Change to end of line
- `C` - Change to end of line (same as c$)
- `r{char}` - Replace single character
- `R` - Replace mode

### Undo/Redo
- `u` - Undo
- `Ctrl+r` - Redo
- `.` - Repeat last command

## Search and Replace

- `/{pattern}` - Search forward
- `?{pattern}` - Search backward
- `n` - Next search result
- `N` - Previous search result
- `*` - Search for word under cursor (forward)
- `#` - Search for word under cursor (backward)
- `:%s/old/new/g` - Replace all occurrences in file
- `:%s/old/new/gc` - Replace all with confirmation
- `:s/old/new/g` - Replace all in current line

## File Operations

- `:w` - Save file
- `:w filename` - Save as filename
- `:q` - Quit
- `:q!` - Quit without saving
- `:wq` or `ZZ` - Save and quit
- `:x` - Save and quit (only if changes made)
- `:e filename` - Open file
- `:r filename` - Insert contents of file
- `:bn` - Next buffer
- `:bp` - Previous buffer
- `:bd` - Delete buffer

## Text Objects

- `iw` - Inner word
- `aw` - A word (includes surrounding whitespace)
- `is` - Inner sentence
- `as` - A sentence
- `ip` - Inner paragraph
- `ap` - A paragraph
- `i"` - Inner quotes
- `a"` - A quotes (includes quotes)
- `i(` or `i)` - Inner parentheses
- `a(` or `a)` - A parentheses (includes parentheses)
- `i{` or `i}` - Inner braces
- `a{` or `a}` - A braces (includes braces)
- `i[` or `i]` - Inner brackets
- `a[` or `a]` - A brackets (includes brackets)

## Marks and Jumps

- `m{letter}` - Set mark
- `'{letter}` - Jump to mark
- `''` - Jump to previous position
- ``.`` - Jump to last edit
- `Ctrl+o` - Jump to older position
- `Ctrl+i` - Jump to newer position

## Windows and Tabs

- `:sp` or `:split` - Horizontal split
- `:vsp` or `:vsplit` - Vertical split
- `Ctrl+w h/j/k/l` - Navigate between windows
- `Ctrl+w w` - Switch between windows
- `Ctrl+w q` - Close window
- `Ctrl+w =` - Equalize window sizes
- `:tabnew` - New tab
- `gt` - Next tab
- `gT` - Previous tab
- `:tabclose` - Close tab

## Visual Mode Commands

- `d` - Delete selection
- `y` - Copy selection
- `c` - Change selection
- `>` - Indent selection
- `<` - Unindent selection
- `=` - Auto-indent selection
- `u` - Lowercase selection
- `U` - Uppercase selection

## Command Mode Shortcuts

- `:!{command}` - Execute shell command
- `:r !{command}` - Insert output of shell command
- `:set number` - Show line numbers
- `:set nonumber` - Hide line numbers
- `:set hlsearch` - Highlight search results
- `:noh` - Clear search highlighting
- `:syntax on` - Enable syntax highlighting
- `:help {topic}` - Get help on topic

## Useful Combinations

- `ciw` - Change inner word
- `diw` - Delete inner word
- `yiw` - Copy inner word
- `ci"` - Change text inside quotes
- `di(` - Delete text inside parentheses
- `va{` - Select text including braces
- `>i{` - Indent text inside braces
- `=G` - Auto-indent from cursor to end of file
