# tmux.conf
Configuracion de tmux  y comandos

# create or add this your ur ~/.tmux.conf
# sudo vim ~/.tmux.conf
#set prefix
set -g prefix C-a
bind C-a send-prefix
unbind C-b

set -g history-limit 100000
set -g allow-rename off
set -g @plugin 'tmux-plugins/tmux-logging'
set -g status-bg colour27
set -g status-fg white

bind-key j command-prompt -p "Join pane from:" "join-pane -s '%%'"
bind-key s command-prompt -p "Send pane to:" "join-pane -t '%%'"

set-window-option -g mode-keys vi

run-shell /opt/tmux-logging/logging.tmux

# next run
# tmux new -s Bounty
# ctrl A + i

# sudo git clone https://github.com/tmux-plugins/tmux-logging /opt/tmux-logging/
# tmux source-file ~/.tmux.conf

# Ctrl A + shift + p
# Ctrl A + , >> rename window
# Ctrl A + " >> dividir pantalla hori
# hold Ctrl A + flecha arriba o bajo >> minimiza o maximiza
# -a C-o     Rotate through the panes                                                                                                                                                        [41/41]
# C-a C-z     Suspend the current client                                                                                                                                                             
# C-a Space   Select next layout                                                                                                                                                                     
# C-a !       Break pane to a new window                                                                                                                                                             
# C-a "       Split window vertically                                                                                                                                                                
# C-a #       List all paste buffers                                                                                                                                                                 
# C-a $       Rename current session                                                                                                                                                                 
# C-a %       Split window horizontally                                                                                                                                                              
# C-a &       Kill current window                                                                                                                                                                    
# C-a '       Prompt for window index to select                                                                                                                                                      
# C-a (       Switch to previous client                                                                                                                                                              
# C-a )       Switch to next client                                                                                                                                                                  
# C-a ,       Rename current window                                                                                                                                                                  
# C-a -       Delete the most recent paste buffer                                                                                                                                                    
# C-a .       Move the current window                                                                                                                                                                
# C-a /       Describe key binding                                                                                                                                                                   
# C-a 0       Select window 0                                                                                                                                                                        
# C-a 1       Select window 1                                                                                                                                                                        
# C-a 2       Select window 2                                                                                                                                                                        
# C-a 3       Select window 3                                                                                                                                                                        
# C-a 4       Select window 4                                                                                                                                                                        
# C-a 5       Select window 5                                                                                                                                                                        
# C-a 6       Select window 6
# C-a 7       Select window 7
# C-a 8       Select window 8
# C-a 9       Select window 9
# C-a :       Prompt for a command
# C-a ;       Move to the previously active pane
# C-a =       Choose a paste buffer from a list
# C-a ?       List key bindings
# C-a C       Customize options
# C-a D       Choose a client from a list
# C-a E       Spread panes out evenly
# C-a L       Switch to the last client
# C-a M       Clear the marked pane
# C-a [       Enter copy mode
# C-a ]       Paste the most recent paste buffer
# C-a c       Create a new window
# C-a d       Detach the current client
# C-a f       Search for a pane                                                                                                                                                                [2/41]
# C-a i       Display window information
# C-a l       Select the previously current window
# C-a m       Toggle the marked pane
# C-a n       Select the next window
# C-a o       Select the next pane
# C-a p       Select the previous window
# C-a q       Display pane numbers
# C-a r       Redraw the current client
# C-a t       Show a clock
# C-a w       Choose a window from a list
# C-a x       Kill the active pane
# C-a z       Zoom the active pane
# C-a {       Swap the active pane with the pane above
# C-a }       Swap the active pane with the pane below
# C-a ~       Show messages
# C-a DC      Reset so the visible part of the window follows the cursor
# C-a PPage   Enter copy mode and scroll up
# C-a Up      Select the pane above the active pane
# C-a Down    Select the pane below the active pane
# C-a Left    Select the pane to the left of the active pane
# C-a Right   Select the pane to the right of the active pane
# C-a M-1     Set the even-horizontal layout
# C-a M-2     Set the even-vertical layout
# C-a M-3     Set the main-horizontal layout
# C-a M-4     Set the main-vertical layout
# C-a M-5     Select the tiled layout
# C-a M-n     Select the next window with an alert
# C-a M-o     Rotate through the panes in reverse
# C-a M-Up    Resize the pane up by 5
# C-a M-Down  Resize the pane down by 5
# C-a M-Left  Resize the pane left by 5
# C-a M-Right Resize the pane right by 5
# C-a C-Up    Resize the pane up
# C-a C-Down  Resize the pane down
# C-a C-Left  Resize the pane left
# C-a C-Right Resize the pane right
# C-a S-Up    Move the visible part of the window up
# C-a S-Down  Move the visible part of the window down


