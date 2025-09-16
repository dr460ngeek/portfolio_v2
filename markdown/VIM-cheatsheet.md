# Vim Cheatsheet (Enhanced)

## Cursor Movement
| Key | Action |
|-----|--------|
| h | Move cursor left |
| j | Move cursor down |
| k | Move cursor up |
| l | Move cursor right |
| 0 | Move cursor to beginning of line |
| ^ | Move cursor to first non-whitespace character of line |
| $ | Move cursor to end of line |
| w | Jump forward to beginning of next word |
| e | Jump forward to end of word |
| b | Jump backward to beginning of word |
| gg | Move cursor to beginning of the file |
| G | Move cursor to end of the file |
| `n`G (or) :`n` | Move cursor to line number `n` (e.g., `5G`) |
| Ctrl-d | Move cursor half-page down |
| Ctrl-u | Move cursor half-page up |
| Ctrl-f | Page forward |
| Ctrl-b | Page backward |

---

## File Management
| Command | Action |
|---------|--------|
| :e filename | Open file for editing |
| :w | Save current buffer to disk |
| :w filename | Save current buffer to `filename` |
| :q | Quit current window (fails if unsaved changes) |
| :wq or ZZ | Save and quit |
| :q! | Quit without saving |
| :wa | Save all buffers |
| :qa | Quit all windows |
| :wqa | Save all and quit |
| :n | Open next file in argument list |
| :prev | Open previous file in argument list |

---

## Editing Commands I (Insert Mode)
| Key | Action |
|-----|--------|
| i | Insert before cursor |
| a | Insert after cursor |
| I | Insert at beginning of line |
| A | Insert at end of line |
| o | Open new line below and insert |
| O | Open new line above and insert |
| gi | Insert at last insertion point |

---

## Editing Commands II (Changes & Deletion)
| Key | Action |
|-----|--------|
| x | Delete character under cursor |
| X | Delete character before cursor |
| dd | Delete the current line |
| D | Delete from cursor to end of line |
| C | Change (delete) to end of line, then insert |
| r + {char} | Replace a single character |
| s | Substitute (delete) character and insert |
| cc | Change (replace) entire line |
| u | Undo last change |
| Ctrl-r | Redo last undone change |
| . | Repeat last command |
| cw | Change word from cursor to end |
| cb | Change word from cursor to beginning |

---

## Copy, Paste, and Indentation
| Key | Action |
|-----|--------|
| yy | Yank (copy) current line |
| y$ | Yank from cursor to end of line |
| yw | Yank word from cursor |
| p | Paste after cursor |
| P | Paste before cursor |
| >> | Indent current line |
| << | Un-indent current line |
| =G | Auto-indent till end of file |

---

## Visual Mode Commands
| Key | Action |
|-----|--------|
| v | Start visual (character-wise) selection |
| V | Start visual (line-wise) selection |
| Ctrl-v | Start visual block selection |
| y | Yank selected text |
| d | Delete selected text |
| c | Change selected text and insert |
| > | Indent selected text |
| < | Un-indent selected text |

---

## Search and Replace
| Command | Action |
|---------|--------|
| /pattern | Search forward for `pattern` |
| ?pattern | Search backward for `pattern` |
| n | Repeat search in same direction |
| N | Repeat search in opposite direction |
| :%s/old/new/g | Replace all occurrences in file |
| :%s/old/new/gc | Replace all occurrences with confirmation |
| :s/old/new/ | Replace first occurrence in current line |
| :noh | Clear search highlighting |

---

## Buffers, Splits, and Tabs
| Command | Action |
|---------|--------|
| :ls | List open buffers |
| :b n | Switch to buffer number `n` |
| :bn | Go to next buffer |
| :bp | Go to previous buffer |
| :bd | Close (delete) current buffer |
| :sp file | Split window horizontally with `file` |
| :vsp file | Split window vertically with `file` |
| Ctrl-w w | Switch between windows |
| Ctrl-w q | Quit current window |
| Ctrl-w h/j/k/l | Move to split in direction (left, down, up, right) |
| :tabe file | Open file in new tab |
| :tabn | Next tab |
| :tabp | Previous tab |
| :tabc | Close current tab |

---

## Macros and Registers
| Command | Action |
|---------|--------|
| qa | Start recording a macro in register `a` |
| q | Stop recording macro |
| @a | Run macro `a` |
| @@ | Repeat last executed macro |
| "ay | Yank into register `a` |
| "ap | Paste from register `a` |
| "+y | Yank to system clipboard (if supported) |
| "+p | Paste from system clipboard |

---

## Marks and Jumps
| Command | Action |
|---------|--------|
| ma | Set mark `a` at cursor position |
| `a | Jump to mark `a` (exact position) |
| 'a | Jump to beginning of line containing mark `a` |
| `` | Jump back to previous cursor location |
| Ctrl-o | Jump to older cursor position in jump list |
| Ctrl-i | Jump to newer cursor position in jump list |

