# .tmux dotfiles

Current setup includes remapping of default escape sequence, remapping of split commands, vim-like remapping of window navigation commands, and more. This is a work in progress.

## Basic commands
**Control-a** Prefix command. Use this to execute other shortcut commands, like toggling a screen split.  
**Control-a |** Split the screen vertically   
**Control-a -** Split the screen horizontally  
**Control-a h** (Alternatively, **Control-a ←**) Move focus to panel left of current panel  
**Control-a l** (Alternatively, **Control-a →**) Move focus to panel right of current panel   
**Control-a k** (Alternatively, **Control-a ↑**) Move focus to panel above of current panel  
**Control-a j** (Alternatively, **Control-a ↓**) Move focus to panel below current panel   
**Control-a Control-h** or **Control-a Control-l** Resize panel horizontally to the right or left, respectively  
**Control-a Control-k** or **Control-a Control-j** Resize panel vertically up or down, respectively  

##For Austin
###Basic use
**Opening a tmux session** `tmux`  
**Viewing open tmux sessions** `tmux ls`  
**Attaching to tmux session** `tmux attach -t <session name>`  
