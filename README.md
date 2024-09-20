# CHEATSHEET
![](ZZZ/ZZZ.jpg)

## MOTIONS
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `UP/DOWN/LEFT/RIGHT` | Move cursor |
| `CTRL-u/ CTRL-d` | Half page up/down |
| `b / w` | Prev/next word |
| `ge / e` | End of previous/next word |
| `0 / $` | Start/end of line |
| `^` | Start of line (non blank) |
| `FCHARACTER / fCHARACTER` | Goto prev/next `CHARACTER` |
| `\| / N\|` | Move to first/N th column |
| `gg / G` | Goto first/last line |
| `:N` | Goto N th line |
| `{ / }` | Goto previous/next empty line |

## INSERT MODE
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `i` | Insert mode |
| `C / cc` | Change to end of/current line |
| `o / O` | Insert below/above the line |

## NORMAL MODE
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `r` | Replace one character |
| `R` | Replace mode |
| `u / Nu` | Undo one/N changes |
| `CTRL-r / n CTRL-r` | Redo one/N changes |
| `J` | Join next line with current |
| `> / <` | Shift text right/left |

## VISUAL MODE
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `v` | Enter visual mode |
| `V` | Enter visual line mode |
| `CTRL-v` | Enter visual block mode |
| `d` | Delete selection |
| `s` | Replace selection |
| `y` | Yank selection |
| `=` | Formats code |
| `dx` | Delete selection |

## CUT and PASTE
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `x` | Delete character |
| `p / P` | Paste before/after |
| `xp` | Swap 2 adjacent characters |
| `dw` | Delete word |
| `dd` | Delete line |
| `ddp` | Swap 2 lines |
| `yy` | Yank line |
| `D` | Delete to end of line |
| `"*p / "+p` | Paste from system clipboard |
| `"*y / "+y` | Paste to system clipboard |

## REPEATING
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `.` | Repeat last command |
| `;` | Repeat latest f, F, t, T |
| `.` | Repeat latest f, F, t, T reversed |
| `&` | Repeat last `:s` |
| `@:` | Repeat a command-line command |

## MACROS
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `qi` | Record macro i |
| `q` | Stop recording macro |
| `@i` | Run macro i |
| `7@i` | Run macro i 7 times |
| `@@` | Repeat last macro |

## OPERATORS
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `d` | Delete |
| `y` | Yank |
| `c` | Change (Delete then insert) |
| `p` | Paste |
| `=` | Formats code |
| `g~` | Toggles case |
| `gU` | Upper case |
| `gu` | Lower case |
| `> / <` | Indent right/left |

### OPERATOR COMBINATIONS
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `dd` | Delete current line |
| `dw` | Delete to next word |
| `db` | Delete to beginning of word |
| `cc` | Change current line |
| `yy` | Yank current line |
| `d/WORD` | Delete until word |
| `dfx` | Delete until `x` char |
| `Ndd` | Delete N lines |
| `dNw` | Delete N words |
| `dNj` | Delete N lines downwards |
| `Nyy` | Yank N lines |
| `ggdG` | Delete complete document |
| `gg=G` | Indent complete document |
| `ggyG` | Copy whole document |
| `ggvG` | Select all text |

## TEXT OBJECTS
| **TEXT OBJECT** | **OBJECT TYPE** |
| --------------- | --------------- |
| `p` | Paragraph |
| `w` | Word |
| `W` | Word surrounded by white spaces |
| `s` | Sentence |
| `[({<` | A [], (), or {} block |
| `])}>` | A [], (), or {} block |
| `'"` | A quoted string |
| `b` | A block [( |
| `B` | A block in [{ |

## SAVE and EXIT
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `:wq / :xx / ZZ` | Save and quit |
| `:wqa` | Write and quit all files |
| `:q! / ZQ` | Force quit |
| `:qa` | Quit all files |
| `:qa!` | Force quit all files |
| `:sav FILE_NAME` | Save current file and start editing `FILE_NAME` |
| `:w !sudo tee %` | Write ot readonly file |

## OTHERS
* `!`
