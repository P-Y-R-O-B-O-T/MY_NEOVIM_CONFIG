# CHEATSHEET
![](ZZZ/ZZZ.jpg)

## MOTIONS
| **KEYMAPPING** | **EFFECT** |
| ---------- | ------ |
| `UP/DOWN,LEFT/RIGHT` | Move cursor |
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
| ---------- | ------ |
| `i` | Insert mode |
| `C / cc` | Change to end of/current line |
| `o / O` | Insert below/above the line |

## NORMAL MODE
| **KEYMAPPING** | **EFFECT** |
| ---------- | ------ |
| `r` | Replace one character |
| `R` | Replace mode |
| `u / Nu` | Undo one/N changes |
| `CTRL-r / n CTRL-r` | Redo one/N changes |
| `J` | Join next line with current |

## SAVE and EXIT
| **KEYMAPPING** | **EFFECT** |
| ---------- | ------ |
| `:wq / :xx / ZZ` | Save and quit |
| `:wqa` | Write and quit all files |
| `:q! / ZQ` | Force quit |
| `:qa` | Quit all files |
| `:qa!` | Force quit all files |
| `:sav FILE_NAME` | Save current file and start editing `FILE_NAME` |
| `:w !sudo tee %` | Write ot readonly file |
