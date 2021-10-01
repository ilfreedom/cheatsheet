# terminal shortcut

- [terminal shortcut](#terminal-shortcut)
  - [screen & tmux](#screen--tmux)
    - [session](#session)
    - [split screen](#split-screen)
    - [window](#window)
    - [copy mode](#copy-mode)
  - [terminator & iterm2](#terminator--iterm2)
    - [tab](#tab)
    - [split window](#split-window)

## screen & tmux

### session

| function                 | screen                                                     | tmux                                   |
| ------------------------ | ---------------------------------------------------------- | -------------------------------------- |
| new session              | screen -S session_name                                     | tmux new -s session_name or C-b Ctrl+c |
| detach session           | C-a d                                                      | C-b d                                  |
| kill session             | C-a  \\                                                    | exit                                   |
| list session             | screen -ls                                                 | tmux ls <br> C-b s                     |
| attach session           | screen -r session_name                                     | tmux a -t session_name or tmux a       |
| attach running session   | screen -x                                                  |                                        |
| switch session           |                                                            |                                        |
| rename session           | C-a :sessionname new <br> screen -S old -X sessionname new | C-b $                                  |
| remote detach session    | screen -d session_name                                     |                                        |
| remote kill session      | screen -X -S session_name quit                             | tmux kill-session -t session_name      |
| kill all session but cur |                                                            | tmux kill-session -a                   |
| remote kill all          |                                                            | tmux kill-server                       |
| clear dead session       | screen -wipe                                               |                                        |

### split screen

| function             | screen                      | tmux                    |
| -------------------- | --------------------------- | ----------------------- |
| split H              | C-a S                       | C-b "                   |
| split V              | C-a \|                      | C-b %                   |
| close cur pane       | C-a X                       | C-b x                   |
| close all but cur    | C-a Q                       |                         |
| go to pane           | C-a tab                     | C-b arrow or o or ⌥ + ⇧ |
| resize the pane      | C-a :resize p%/max/min/-b = | C-b follow by  ⌥ + ⇧    |
| toogle pane zoom     |                             | C-b z                   |
| switch pane position |                             | C-b {/}                 |

### window

| function          | screen          | tmux             |
| ----------------- | --------------- | ---------------- |
| create window     | C-a c           | C-b c            |
| switch window     | C-a n/p C-a 0-9 | C-b n/p  C-b 0-9 |
| switch two window | C-a C-a         | C-b l            |
| switch by order   | C-a [Space]     |                  |
| rename window     | C-a A           | c-b ,            |
| lock cur window   | C-a x           |                  |
| list all window   | C-a " or C-a w  | C-b w            |
| kill window       | C-a k           | C-b &            |

### copy mode

| function                       | screen       | tmux              |
| ------------------------------ | ------------ | ----------------- |
| switch copy mode               | C-a [ or esc | C-b [, q for quit |
| page up/down by half of screen | Ctrl - u/d   |                   |
| page up/dwon by a full screen  | Ctrl - b/f   |                   |

## terminator & iterm2

### tab

| function  | iterms                  | terminator           |
| --------- | ----------------------- | -------------------- |
| New Tab   | ⌘ + T                   | ctrl+shif+T          |
| Close Tab | ⌘ + W                   |                      |
| Go to Tab | ⌘ + Number or ⌘ + Arrow | Ctrl+PageUp/PageDown |

### split window

| function                         | iterms                    | terminator           |
| -------------------------------- | ------------------------- | -------------------- |
| **Paste history**                | command + shift + h       |                      |
| Find                             | ⌘ + F                     |                      |
| Undo                             | Ctrl -                    |                      |
| Split Window V                   | ⌘ + D                     | Ctrl+Shift+O         |
| Split Window H                   | ⌘ + Shift + D             | Ctrl+Shift+E         |
| Go to Split                      | ⌘ + ⌥ + ⇧                 | Alt + Arrow          |
| Go to Split Pane by Order        | ⌘ + ] , ⌘ + [             |                      |
| resize the split                 | ⌘ ^ ⇧                     | Ctrl+Shift+Left/Down |
| Close current Pane               | ⌘ + w                     |                      |
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
