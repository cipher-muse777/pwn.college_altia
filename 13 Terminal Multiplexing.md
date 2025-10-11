# Launching Screens 

**FLAG:** pwn.college{4z5oZFV5JjmeUT_B4aVPpDlXTUJ.0VN4IDOxwCMyAzNzEzW}
i first executed screen and then exited using ctrl+d to exit and obtained the flag

### What i learned 
how we can use screen command to create virtual terminals inside our terminal. It's somewhat like having multiple browser tabs, but for your command line

# Detaching And Attaching 

**FLAG:** pwn.college{sKpr8t8mfA-eOcPMobEs_CEfSrF.0lN4IDOxwCMyAzNzEzW}
i first executed screen command then i detached using ctrl+A and then d and then ran the command /challenge/run and then reattched using screen -r to obtain the flag

### What i learned 
how we can detach from screen using ctrl+A and then d and reattach using screen -r 

# Finding Sessions

**FLAG:** pwn.college{8-N5ZyThTXxgtQzcsctNGA-jb7o.01N4IDOxwCMyAzNzEzW}
i first executed screen -ls to see the screen activity and then used screen -r with the PID for each session till i found the flag 

### What i learned 
how we can use screen -ls to view the screen activity

# Switching Windows 

**FLAG:** pwn.college{MfzOGrfN7klZIC2Yxw3CxzRK78J.0FO4IDOxwCMyAzNzEzW}
i first executed screen -r and then used ctrl+A then 0 and obtained the flag

### What i learned 
Ctrl-A c - Creates a new window
Ctrl-A n - Next window
Ctrl-A p - Previous window
Ctrl-A 0 through Ctrl-A 9 - Jump directly to window 0-9
Ctrl-A " - bring up a selection menu of all of the windows

# Detaching And Attaching (tmux)

**FLAG:** pwn.college{Uy-a8gs6nMvxKc3Rn0zL8c7PXSd.0VO4IDOxwCMyAzNzEzW}
i first executed tmux and then detached using ctrl+B then d then ran /challenge/run and then i reattched usinf tmux a to obtain the flag

### What i learned 
how we can launch using tmx (terminal multiplexer), tmux ls to list sessions, tmux a to reattach to session and ctrl+B then d to detach

# Switching Windows (tmux)

**FLAG:** pwn.college{sJm8Z4jxlLzgH7oszaaN5DvOzNs.0FM5IDOxwCMyAzNzEzW}
i first executed tmux a to reattach then did ctrl+B 0 to obtain the flag

### What i learned 
Ctrl-B c - Create a new window
Ctrl-B n - Next window
Ctrl-B p - Previous window
Ctrl-B 0 through Ctrl-B 9 - Jump to window 0-9
Ctrl-B w - See a nice window picker



