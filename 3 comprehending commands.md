# Cat Not The Pet But The Command

**FLAG:** pwn.college{YyxnF03cnl3vgLaSOlTO8D5XCrY.QXxcTN0wCMyAzNzEzW}
i put cat flag and it showed me the flag 

### What i learned 
cat command reads out the file

# Catting Absolute Path
**FLAG:** pwn.college{8rWIv0sZ-VlILaxuzygd89lua69.QX5ETO0wCMyAzNzEzW}
i put cat /flag and it showed me the flag 

### What i learned 
cat command can read absolute path

# More Catting Practice 

**FLAG:** pwn.college{Iv_Cddl9uLN3u2wcxcVWoBsAyfT.QXwITO0wCMyAzNzEzW}
since we cant use cd here i typed in cat /lib/x86_64-linux-gnu/valgrind/flag as already showed in terminal and got the flag

### What i learned
You can specify all sorts of paths as arguments to cat command and we can read files without actually openeing it using cd command

# Grepping for A Needle In A Haystack

**FLAG:** pwn.college{EQm4elhhDrNh89X6UafdqOgYgwd.QX3EDO0wCMyAzNzEzW}
i typed in grep pwn.college /challenge/data.txt so i got the flag

### What i learned 
grep command searches the file for lines of text containing a particular string and print them to the console 

# Comparing Files 

**FLAG:** pwn.college{oAV9zPnjNEZIWMlKz4afLgaJpMj.01MwMDOxwCMyAzNzEzW}
i first opened the /challenge directory using cd and then used diff command to find the difference between the two files and since it was an additional line with the flag it was shown

### What i learned 
diff command shows us the difference between two files, whether it is addition or change eg: 1a2 means after line 1 of file1 add line 2 of file2 and 2c2 means line 2 od file1 is changed with line2 of file2

# Listing Files

**FLAG:** pwn.college{Aozx5o7c2lhh5mFdM6_T1sqfNDg.QX4IDO0wCMyAzNzEzW}
i first opened /challenge directpry using cd and then used ls to list the files then i replaced run with 11338-renamed-run-13615 and executed /challenge/11338-renamed-run-13615 hence obtaining the flag

### What i learned 
how using ls i can list the files in a directory

# Touching Files 

**FLAG:** pwn.college{cxzmqdTtG4uV0uBB-si0x0OzasH.QXwMDO0wCMyAzNzEzW}
i first opened /tmp directory using cd and then created two files pwn and college and then executed /challenge/run and hence otained the flag

### What i learned 
how i can create files using touch command

# Removing Files

**FLAG:** pwn.college{4itHnAKAya_88PNawUxmYKirkNx.QX2kDM1wCMyAzNzEzW}
i deleted file using rm and then executed /challenge/check to obtain the flag

### What i learned 
how i can delete files using rm command

# Moving Files

**FLAG:** pwn.college{8q04GhF5qE8yZvn-O2W2jN4Sep0.0VOxEzNxwCMyAzNzEzW}
i moved the content in /flag file to /tmp/hack-the-planet using mv and then executed /challenge/check to obtain the flag

### What i learned 
how i can move the contents of a file to an another file using mv command

# Hidden Files 

**FLAG:** pwn.college{I8iXOhmVbQ81-_ZazV0expHmkiq.QXwUDO0wCMyAzNzEzW}
i used cd to open the / directory and then used ls -a to find the flag and then used cat to read the flag

### What i learned 
we can use ls -a to find the hidden files in a dirctory

# An Epic Filesystem Quest

**FLAG:** pwn.college{oHob38CoesyftFK3lQdMif_bhCW.QX5IDO0wCMyAzNzEzW}
i started using cd / then i used ls to list the files then i used cat to read DISPATCH then i opened /usr/share/locale/am/LC_MESSAGES then i used ls then i read SPOILER then i listed the files of /opt/linux/linux-5.4/include/config/x86/64/acpi without opening due to instructions and then read the file NUGGET-TRAPPED. then i opened /usr/share/javascript/mathjax/jax/output/SVG/fonts/Gyre-Pagella/Latin ls -a to find .BLUEPRINT then i read it to open /opt/linux/linux-5.4/drivers/usb/host then i listed the files and then read NOTE. then i opened /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/nvkm and then ls -a to find .TIP to find /usr/share/racket/pkgs/gui-pkg-manager-lib/pkg/gui which i then opened and ls -a to find CLUE then i read it and opened /usr/share/racket/pkgs/typed-racket-compatibility/typed/scheme/base/no-check/lang/compiled and then ls -a to find HINT. i then opened /usr/lib/python3/dist-packages/sage/coding/source_coding/__pycache__ and ls -a to find .SNIPPET and finally founf the flag.

### What i learned 
its about applying all that you know into a problem and stay focused

# Making Directories

**FLAG:** pwn.college{slBygbnRUWY4yfhOBTB46TSjWU6.QXxMDO0wCMyAzNzEzW}
i first used mkdir to form /tmp/pwn and then used touch command to make the college file in it then executed /challenge/run to get the flag 

### What i learned 
we can use mkdir command to create directories

# Finding Files 

**FLAG:** pwn.college{AOBuqaVegWaDEqBA4lnnhqU794J.QXyMDO0wCMyAzNzEzW}
i first used find / -name flag then used cat command on each element that was found till i found the flag

### What i learned 
we can use find command to easily find files and directories

# Linking Files 

**FLAG:** pwn.college{QaOpIE3ue4apn9hvrxIYXQ4Ulzh.QX5ETN1wCMyAzNzEzW}
i first tried linking /flag and /home/hacker/not-the-flag so it showed file already exists so i used rm command to delete /home/hacker/not-the-flag and then linked them. then i put the command /challenge/catflag to obtain the flag 

### What i learned 
we can use ln -s command to link 2 files 
