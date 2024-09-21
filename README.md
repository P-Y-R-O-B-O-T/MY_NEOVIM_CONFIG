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
| `CTRL-o` | Get into normal mode temporarily and run commands |

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
| `dfCHARACTER` | Delete until `x` char |
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

### TEXT OBJECT OPERATIONS
| **KEYMAPPING** | **OBJECT** |
| -------------- | ---------- |
| `vi"` | Select inner quotes `"..."` |
| `va"` | Select quotes `"..."` |
| `vi[` | Select inner brackets `[...]` |
| `va[` | Select brackets `[...]` |
| `viw` | Select inner word |
| `vip` | Select inner paragraph |
| `vipip` | Select more paragraph |
| `diw` | Delete inner word |
| `dis` | Delete inner sentence |
| `di"` | Delete in quotes |
| `da"` | Delete in quotes (including quotes) |
| `dip` | Delete a paragraph |
| `ciw` | Change inner word |
| `ci"` | Change inner quotes |
| `cit` | Change inner tags (HTML) |
| `cip` | Change inner paragraph |
| `yip` | Yank inner paragraph |
| `yap` | Yank paragraph (including newline) |

## SEARCH and REPLACE
### SEARCH
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `/TEXT` | Search forward |
| `/TEXT\c` | Search forward case sensitive |
| `?TEXT` | Search backward |
| `n` | Next matching search pattern |
| `N` | Previous match |
| `*` | Search for current word forward |
| `#` | Search for current word backward |

### RANGES
| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `%` | Entire file |
| `’<,’>` | Current selection |
| `5` | Line 5 |
| `5,10` | Lines 5 to 10 |
| `$` | Last line |
| `2,$` | Lines 2 to Last |
| `.` | Current line |
| `,3` | Next 3 lines |
| `-3,` | Forward 3 lines |

### FLAGS
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `g` | Replace all occurrences |
| `i` | Ignore case |
| `I` | Don't ignore case |
| `c` | Confirm each substitution |

### REPLACE LINE
> [!TIP]
> FORMAT : `:[range]s/{pattern}/{str}/[flags]`

| **KEYMAPPING** | **EFFECT** |
| -------------- | ---------- |
| `:s/old/new` | Replace first |
| `:s/old/new/g` | Replace all |
| `:s/\vold/new/g` | Replace all with regex |
| `:s/old/new/gc` | replace all (Confirm) |
| `:s/old/new/i` | Ignore case replace first |
| `:N,Ms/old/new/g` | Replace between lines N-M |

### REPLACE FILE
> [!TIP]
> FORMAT : `:%s/{pattern}/{str}/[flags]`

| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `:%s/old/new` | Replace first |
| `:%s/old/new/g` | Replace all |
| `:%s/old/new/gc` | Replace all (Confirm) |
| `:%s/old/new/gi` | Replace all (ignore case) |
| `:%s/\vold/new/g` | Replace all with regex |

### GLOBAL COMMAND
> [!TIP]
> FORMAT : `:[range]g/{pattern}/[command]`

| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `:g/foo/d` | Delete lines containing foo |
| `:g!/foo/d` | Delete lines not containing foo |
| `:g/^\s*$/d` | Delete all blank lines |
| `:g/foo/t$` | Copy lines containing foo to EOF |
| `:g/foo/m$` | Move lines containing foo to EOF |
| `:g/^/m0` | Reverse a file |
| `:g/^/t.` | Duplicate every line |

### SUBSTITUTION EXPRESSION (MAGIC)
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `& \| \0` | Replace with the whole matched |
| `\1...\9` | Replace with the group 0-9 |
| `\u` | Uppercase next letter |
| `\U` | Uppercase following characters |
| `\l` | Lowercase next letter |
| `\L` | Lowercase following characters |
| `\e` | End of \u, \U, \l and \L |
| `\E` | End of \u, \U, \l and \L |

#### EXAMPLES
| **EXPRESSION** | **EFFECT** |
| -------------- | ---------- |
| `:s/a\|b/xxx\0xxx/g` | Modifies "a b" to "xxxaxxx xxxbxxx" |
| `:s/test/\` | Modifies "test" to "TEST FILE" |
| `:s/\(test\)/\U\1` | Modifies "test" to "TEST file" |
| `:s/\v([abc])([efg])/\2\1/` | Modifies "af fa bg" to "fa fa gb" |
| `:s/\v\w+/\u\0/g` | Modifies "bla bla"  to "Bla Bla" |
| `:s/\v([ab])\|([cd])/\1x` | Modifies "a b c d"  to "ax bx x x" |
| `:%s/.*/\L` | Modifies "HTML" to "html" |
| `:s/\v<(.)(\w*)/\u\1\L\2` | Make every first letter of a word uppercase |
| `:%s/^\(.*\)\n\1/\` | Remove duplicate lines |
| `:%s/<\/\=\(\w\+\)\>/\U&` | Convert HTML-Tags to uppercase |
| `:g/^pattern/s/$/myte` | Find and append text to the end |
| `:g/pattern/nor` | Run a macro on matching lines |
| `/^\(.*\)\(\r\?\n\1\)\` | View the duplicates lines |
| `/\v^(.*)(\r?\n\1)` | View the duplicates lines (very magic) |
| `:v/./,/./` | Compress blank lines into a blank line |
| `:g/<p1>/,/<p2>` | Delete inclusively from `<p1>` to `<p2>` |

## MISCELLANEOUS
### CASE
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `vU` | Uppercase character |
| `vu` | Lowercase character |
| `~` | Toggle case character |
| `viw` | Uppercase word |
| `viw` | Lowercase word |
| `viw` | Toggle case word |
| `VU / gUU` | Uppercase line |
| `Vu / guu` | Lowercase line |
| `V~ / g~~` | Toggle case line |
| `gggUG` | Uppercase all text |
| `ggguG` | Lowercase all text |
| `ggg~G` | Toggle case all text |

### JUMPING
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `CTRL-` | Go back to previous |
| `CTRL-i` | Go forward |
| `gf` | Go to file in cursor |
| `ga` | Display hex, ascii value |

### NAVIGATING
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `%` | Nearest/matching `{[()]}` |
| `[( \| [{` | Previous ( or { |
| `]) \| ]{` | Next ) or } |
| `[m` | Previous method start |
| `[M` | Previous method end |

### COUNTERS
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `CTRL-a` | Increase number |
| `CTRL-x` | Decrease number |

### FORMATTING
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `:ce N` | Center lines between N columns |
| `:ri N` | Right-align lines at N columns |
| `:le` | Left-align lines |


### TAGS
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `:tag CLASSNAME` | Jump to first definition of Classname |
| `CTRL-]` | Jump to definition |
| `g]` | See all definitions |
| `CTRL-t` | Go back to last tag |
| `CTRL-o / CTRL-i` | Back/forward |
| `:tselect CLASSNAME` | Find definitions of Classname |
| `:tjump CLASSNAME` | Find definitions of Classname (auto-select 1st) |

### CALCULATOR
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| `CTRL-r = 7*7` | Shows the result |
| `CTRL-r = 10/2` | Shows the result |

### MARKS
| **KEYMAPPINGS** | **EFFECT** |
| --------------- | ---------- |
| ``` `^ ``` | Last position of cursor in insert mode |
| ``` `. ``` | Last change in current buffer |
| ``` `" ``` | Last exited current buffer |
| ``` `0 ``` | In last file edited |
| ``` '' ``` | Back to line in current buffer where jumped from |
| ``` `` ``` | Back to position in current buffer where jumped from |
| ``` `[ ``` | To beginning of previously changed or yanked text |
| ``` `] ``` | To end of previously changed or yanked text |
| ``` `< ``` | To beginning of last visual selection |
| ``` `> ``` | TO end of last visual selection |
| ``` mCHARACTER ``` | Mark this cursor position as `CHARACTER` |
| ``` `CHARACTER ``` | Jump to the cursor position `CHARACTER` |
| ``` 'CHARACTER ``` | Jump to the beginning of the line with position `CHARACTER` |
| ``` d'CHARACTER ``` | Delete from current line to line of mark `CHARACTER` |
| ``` d`CHARACTER ``` | Delete from current position to position of mark `CHARACTER` |
| ``` c'CHARACTER ``` | Change text from current line to line of `CHARACTER` |
| ``` y`CHARACTER ``` | Yank text from current position to position of `CHARACTER` |
| `:marks` | List all current marks |
| `:delm CHARACTER` | Delete mark `CHARACTER` |
| `:delm a-d` | Delete marks a, b, c, d |
| `:delm abc` | Delete marks a, b, c |

## REGISTERS
| **KEYMAPPING** | **KEYMAPPING** |
| -------------- | -------------- |
| `:reg` | See all registers and their content |
| `REGISTERp` | Paste from that register |
| `REGISTERy` | Yank to that register |
| `REGISTERd` | Delete to that register |

### AVAILABLE REGISTERS ARE
* **UNNAMED REGISTERS**: `""` Filled when we delete using commands or yank something
* **STACK REGISTERS**: `"0`, `"1`, `"2`, `"3`, `"4`, `"5`, `"6`, `"7`, `"8`, `"9`
    - `"0`: Used to yank by default
    - `"1`: Used by delete and change by default
* **NAMED REGISTERS**: `"CHARACTER`, Filled when we explicitly tell vim to use
* **SYSTEM CLIPBOARD REGISTERS**: `"+` and `"*`, Have synchronization between system clipboard
* **SMALL DELETE REGISTER**: `"-`, Contain small deletions
* **FILE REGISTER**: `"%`, Contains file name
* **ALTERNATE FILE REGISTER**: `"#`, Contains alternate file name
* **EXPRESSION REGISTER**: `"=`, Stores vim expressions
* **READ ONLY REGISTER**:
    - `":`: Stores the last command executed
    - `".`: Stores last inserted text
* **LAST SEARCH PATTERN REGISTER**: `"/`, Stores last searched pattern
* **BLACK HOLE REGISTER**: `"_`, nothing happens when we write to this and nothing is returned when we read it

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

## TIPS and TRICKS
> [!TIP]
> ### COMMENT TOGGLE
> * Select text in visual mode
> * Then hit `LEADER /`

> [!TIP]
> ### REPLAY CHANGES / REPLACE WORDS
> * Search for the word/pattern
> * Run change in word command `ciw`, write the changes `ESC`
> * Press `n`
> * Press `.` to repeat the last command and changes

> [!TIP]
> ### SPELL CHECK
> * `:set spell` and `:set nospell`

## OTHERS
* `!`
* `/\v\d+`
