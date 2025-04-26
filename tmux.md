# tmux
### terminal inside terminal

## create a new session with name
``` 
tmux new -s <session_name>
```
## list active of session 
``` 
tmux ls
```
## detach session
``` 
ctrl + b  d
```
## attach specific session
``` 
tmux a  -t <session_name>
```
## remove specific session
``` 
tmux kill-session -t <session name>
```
| Option | Meaning | When you use it |
|:------|:--------|:----------------|
| `-s`  | Source (new session) | When creating something new |
| `-t`  | Target (existing session) | When referring to something that already exists |


| Keybinding      | Action                | Description                                               |
|:----------------|:----------------------|:----------------------------------------------------------|
| `ctrl + b %`   | Split Vertical      | Splits the tmux window vertically  |
| `ctrl + b "`   | Split Horizontal    | Splits the tmux window horizontally|
| `ctrl + b Q` + `0`/`1` | Select Pane by Number | Shows pane numbers; press number to jump to that pane    |
| `ctrl + b c`    | Create New Window      | Opens a new window (like a new tab)                       |
| `ctrl + b n`    | Next Window            | Switches to the next window                               |
| `ctrl + b ,`    | Rename Current Window  | Renames the current window                                |
| `ctrl + b w`    | List Windows           | Lists all windows to pick one                             |
| `ctrl + b x`    | Kill Pane              | Closes (kills) the current pane                           |
| `ctrl + b, ctrl + +`| zooming/resizing panes:          |                                             |