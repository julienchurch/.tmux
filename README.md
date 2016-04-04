# .tmux dotfiles

Current setup includes remapping of default escape sequence, remapping of split commands, vim-like remapping of window navigation commands, and more. This is a work in progress.

## Basic commands

**Prefix command** `Control-a`  
Use this command to execute other shortcut commands.  
**Split screen vertically** `Control-a |`  
Makes two panes appear side-by-side in the tmux session.  
**Split screen horizontally** `Control-a -`  
Makes two panes appear on top of one another in the tmux session.  
**Focus left** `Control-a h` (Alternatively `Control-a ←`)  
Puts focus on the pane to the left of the current pane  
**Focus right** `Control-a l` (Alternatively `Control-a →`)  
Puts focus on the pane to the right of the current pane  
**Focus above** `Control-a k` (Alternatively `Control-a ↑`)  
Puts focus on the pane above the current pane  
**Focus below** `Control-a j` (Alternatively `Control-a ↓`)  
Puts focus on the pane below the current pane  
**Resize** `Control-a Control-<directional key>`  
Where `<directional key>` can be any of the following values:  
* `h`: resize horizontally to the left  
* `l`: resize horizontally to the right   
* `k`: resize vertically upwards   
* `j`: resize vertically downwards   
**NB**: This command is tricky at first. You have to hold down `Control` through the entire sequence. Don't release it between hitting the prefix key `a` and the directional keys.   

##For Austin
###Basic use
**Opening a tmux session** `tmux`  
**Viewing open tmux sessions** `tmux ls`  
**Attaching to tmux session** `tmux attach -t <session name>`  
