# Changing File Ownership 

**FLAG:** pwn.college{U2YOZGhwfwkmIeSk6NehuGeLfHf.QXxEjN0wCMyAzNzEzW}
i first did chown hacker /flag to shift the ownership then ran the command cat /flag to obtain the flag 

### What i learned 
how we can change ownership by using the command chown username file

# Groups And Files 

**FLAG:** pwn.college{Anc40alpxMKb4JPZR4PSR-a4V9l.QXxcjM1wCMyAzNzEzW}
i first did chgrp hacker /flag to change the group ownership and then ran the command cat /flag to obtain the flag

### What i learned 
how we can change the group ownership by using the command chgrp groupname file. how id command shows u what all groups you're part of. how /dev/f0 is a device file that lets programs read from or write to the framebuffer which is a chunk of memory that holds the pixel data for what’s currently displayed on your screen.

# Fun With Group Names

**FLAG:** pwn.college{8xHk0pDEkLBoBermeGXjvvVwETM.QXycjM1wCMyAzNzEzW}
i first used the id command to figure out which all groups hacker is in. then figured it was grp22729 and did the command chgrp grp22729 /flag then ran cat /flag to obtain the flag.

### What i learned 
how id shows which all groups user is in 

# Changing Permissions 

**FLAG:** pwn.college{oteG2685yEye06vc1HzVe0sgZB4.QXzcjM1wCMyAzNzEzW}
i first used chmod u+r command, then u+rw  but kept on getting permission denied to read the flag and then i realised i had to enable for all users so i used used chmod a+rwx /flag to obtain the flag 

### What i learned 
how r-  user/group/other can read the file (or list the directory), w- user/group/other can modify the files (or create/delete files in the directory), x- user/group/other can execute the file as a program (or can enter the directory, e.g., using cd) and - refers to nothing.  rw-r--r-- means how the how user can read and write and group and all the other users can only read. HOW WE CAN CHANGE PERMISSIONS by usinf chmod [OPTIONS WHICH EITHER BE u/g/a/o (+/- to add or remove respectively) r/w/x  FILENAME. 

# Executable Files 

**FLAG:** pwn.college{4gvuYGaQdAoIpEN7rCsMAwQu5GK.QXyEjN0wCMyAzNzEzW}
i first used the command chmod a+x /challenge/run to make it executable and then used /challenge/run command to obtain the flag

### What i learned 
how using a+x gives all users executing permission for the particular program 

# Permission Tweaking Practice 

**FLAG:** pwn.college{MssYTIBDSE7IZQDp8JROyBp3nty.QXwEjN0wCMyAzNzEzW}
i executed 1.chmod ug+wx /challenge/pwn, 2.chmod go-r /challenge/pwn, 3.chmod o+x /challenge/pwn, 4.chmod go-rwx /challenge/pwn, 5.chmod u-x /challenge/pwn, 6.chmod uo+x /challenge/pwn, 7.chmod g+rwx /challenge/pwn, 8.chmod ug-r /challenge/pwn. THEN FINALLY i did chmod a+rwx /flag then did cat /flag to obtaint the flag

### What i learned 
how we need to be very observant and properly concentrate while running commands 

# Permission Setiing Practice 

**FLAG:** pwn.college{8-UQTWMo8hRJiLDMqQa8j2OEEb5.QXzETO0wCMyAzNzEzW}
i executes 1.chmod u=rx,g=wx,o=x /challenge/pwn, 2.chmod u=-,g=rwx,o=- /challenge/pwn, 3.chmod u=r,g=rx,o=x /challenge/pwn, 4.chmod u=w,g=rw,o=x /challenge/pwn, 5.chmod u=x,g=rw,o=w /challenge/pwn, 6.chmod u=rx,g=r,o=rw /challenge/pwn, 7.chmod u=r,g=wx,o=w /challenge/pwn, 8.chmod u=rwx,g=rx,o=rw /challenge/pwn, AND THEN FINALLY I DID chmod a=rwx /flag and then ran cat /flag to obtain the flag 

### What i learned 
how we can set permissions overwriting the previous by using chmod u/g/o/a=r/w/x filename AND NO SPACES BETWEEN THEM THE COMMAS

# The SUID Bit

**FLAG:**
