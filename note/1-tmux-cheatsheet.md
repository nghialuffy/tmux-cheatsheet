# Tmux shortcuts & cheatsheet

## How to press <prefix> key in tmux?
```
1. Press <Ctrl> and <b> in the same time
2. Release <Ctrl> and <b>
3. Press shortcuts keys
```

## Cheatsheet
```
- start new tmux: tmux
- start new tmux with session name: tmux new -s <session-name>
- attach: tmux a 
- attach to named: tmux a -t <session-name>
- list sessions: tmux ls
- kill session: tmux kill-session -t <session-name>
```
  
## List all shortcuts

### Sessions
```
:new            start new session
:new -s <name>  start new session with name
s               switch between two session
$               rename session
d               detach
(               move to previous session
)               move to next session
```
### Windows
```
c   create window
w   list windows
n   next window
p   previous window
f   find window
,   name window
&   kill window
```
### Panes
```
%  vertical split
"  horizontal split

o  swap panes
q  show pane numbers
x  kill pane
+  break pane into window (e.g. to select text by mouse to copy)
-  restore pane from window
⍽  space - toggle between layouts
<prefix> q (Show pane numbers, when the numbers show up type the key to goto that pane)
<prefix> { (Move the current pane left)
<prefix> } (Move the current pane right)
<prefix> z toggle pane zoom
```

### Copy - Paste
```
Ctrl b [    enter copy mode
Ctrl b ]    paste to tmux terminal
space       start selection
enter       copy selection
shift v (V) select row
y           select
shift y (Y) copy selection
q           quit copy mode
```
### Misc
```
d  detach
t  big clock
?  list shortcuts
:  prompt
```


### Resizing Panes

```
PREFIX : resize-pane -D (Resizes the current pane down)
PREFIX : resize-pane -U (Resizes the current pane upward)
PREFIX : resize-pane -L (Resizes the current pane left)
PREFIX : resize-pane -R (Resizes the current pane right)
PREFIX : resize-pane -D 20 (Resizes the current pane down by 20 cells)
PREFIX : resize-pane -U 20 (Resizes the current pane upward by 20 cells)
PREFIX : resize-pane -L 20 (Resizes the current pane left by 20 cells)
PREFIX : resize-pane -R 20 (Resizes the current pane right by 20 cells)
PREFIX : resize-pane -t 2 20 (Resizes the pane with the id of 2 down by 20 cells)
PREFIX : resize-pane -t -L 20 (Resizes the pane with the id of 2 left by 20 cells)
```
