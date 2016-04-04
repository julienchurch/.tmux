# .tmux dotfiles

Current setup includes remapping of default escape sequence, remapping of split commands, vim-like remapping of window navigation commands, and more. This is a work in progress.

## Basic commands remapped from default

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
Two of the biggest things tmux is useful for is conserving screen real estate and for being able to save what you're doing. If you shell into a server and open tmux, the next time you shell in you don't have to reopen all the programs from last time. Your old tmux session will still be running, and if you reattach to it, all your work will still be there. You can pick up where you left of without skipping a beat. This is also how I stay logged into IRC persistently: it's just running in a tmux session in the background that I reattach to.

###Basic useage

**Opening a tmux session** `tmux`  
**Viewing open tmux sessions** `tmux ls`  
**Attaching to tmux session** `tmux attach -t <session name>`  
**Renaming a tmux session** `tmux rename -t <old session name> <new session name>`  
**Killing a tmux session** `tmux kill-session -t <session name>`  
**Killing a pane in your current session** `Control-a x y`  
(Technically, `Control-a x` brings up a dialog at the bottom of the screen and you confirm whether you want to close with `y`/`n`.)  

###How2get

1. `cd` into your home directory on your server (`cd` with no arguments is actually the shortcut for this, btw) and `git clone https://github.com/julienchurch/.tmux`. 
2. `cd` into the new directory and `./bootstrap.sh`; this just creates a symbolic link in your home directory to the config file in `.tmux`. (I do this because it's way easier to manage, share, and reuse dotfiles in new servers/machines with Git.)
3. `tmux` and check it out.

