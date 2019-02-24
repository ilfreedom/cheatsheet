
## screen & tmux

### session
| function               | screen                    | tmux                              |
| ---------------------- | ------------------------- | --------------------------------- |
| new session            | screen -S session_name    | tmux new -s session_name          |
| detach session         | C-a d                     | C-b d                             |
| kill session           | C-a  \\                   |                                   |
| list session           | screen -ls                | tmux ls                           |
| attach session         | screen -r session_name    | tmux a -t session_name or tmux a  |
| attach running session | screen -x                 |                                   |
| remote detach session  | screen -d session_name    |                                   |
| remote kill session    | screen -X -S session quit | tmux kill-session -t session_name |
| remote kill all        |                           | tmux kill-server                  |
| clear dead session     | screen -wipe              |                                   |

### split
| function        | screen                      | tmux           |
| --------------- | --------------------------- | -------------- |
| split H         | C-a S                       | C-b "          |
| split V         | C-a \|                      | C-b %          |
| remove cur pane | C-a X                       |                |
| go to splic     | C-a tab                     | C-b arrow or o |
| move the pane   | C-a :resize p%/max/min/-b = | C-b {/}        |


### window
| function          | screen          | tmux             |
| ----------------- | --------------- | ---------------- |
| create window     | C-a c           | C-b c            |
| switch window     | C-a n/p C-a 0-9 | C-b n/p  C-b 0-9 |
| list all window   | C-a w           | C-b w            |
| kill window       | C-a K           | C-b &            |
| switch two window | C-a C-a         | C-b l            |

## terminator & iterm2

### tab

| function  | iterms                  | terminator           |
| --------- | ----------------------- | -------------------- |
| New Tab   | ⌘ + T                   | ctrl+shif+T          |
| Close Tab | ⌘ + W                   |                      |
| Go to Tab | ⌘ + Number or ⌘ + Arrow | Ctrl+PageUp/PageDown |

### split

| function                         | iterms                    | terminator           |
| -------------------------------- | ------------------------- | -------------------- |
| **Paste history**                | command + shift + h       |                      |
| Find                             | ⌘ + F                     |                      |
| Undo                             | Ctrl -                    |                      |
| Split Window V                   | ⌘ + D                     | Ctrl+Shift+O         |
| Split Window H                   | ⌘ + Shift + D             | Ctrl+Shift+E         |
| Go to Split                      | ⌘ + Option + Arrow        | Alt + Arrow          |
| Go to Split Pane by Order        | ⌘ + ] , ⌘ + [             |                      |
| Go to head/tail                  | Ctrl + A, Ctrl + E        |                      |
| Move forward/backward word       | Option + F/B or Esc + F/B |                      |
| Del cur char                     | Ctrl + D                  |                      |
| Del backward char                | Ctrl + H                  |                      |
| Del pre word                     | Ctrl + W                  |                      |
| Del until tail                   | Ctrl + K                  |                      |
| Del until head                   | Ctrl + U                  |                      |
| Copy Mode                        | Shift + ⌘ + C             |                      |
| Char Selection Mode in Copy Mode | Ctrl + V                  |                      |
| Move cursor in Copy Mode         | vim motions               |                      |
| Copy text in Copy Mode           | Ctrl + K                  |                      |
| move the split windows           |                           | Ctrl+Shift+Left/Down |
|                                  |                           |                      |