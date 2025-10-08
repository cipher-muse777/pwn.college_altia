# Learning from Documentation

**FLAG:** pwn.college{oIEKkRCrS3xUk2sUzTbZZvlB67J.QX0ITO0wCMyAzNzEzW}
i used /challenge/challenge with --giveflag therefore obtained flag

### What i learned
how arguments give proper specification to some commands

# Learning Complex Documentation 

**FLAG:** pwn.college{46ufIfAZhw6eUaAYDolXdK4AKNp.QX1ITO0wCMyAzNzEzW}
i used /challenge/challenge --printfile /flag to obtain the flag

### What i learned 
how arguments give proper specification to some commands and --printfile helped me print arbitrary files to the terminal

# Reading Manuals 

**FLAG:** pwn.college{M-fTl4xumls3v72-XfgkBzta4kX.QX0EDO0wCMyAzNzEzW}
i first used man challenge to read the description and details about /challenge/challenge then i used the github link and read the code there so i realised i need -- (some 6 letters) (some 3 numbers) then when i compared this to the stuff written in the manual i saw that --flxuml NUM and then if NUM is 437 flag will be printed so i typed in /challenge/challenge --flxuml 437 and obtained the flag 

### What i learned
i learned how i can use man command to get the description about how to use different commands 

# Searching Manuals 

**FLAG:** pwn.college{IX2uNVWGCDBH8WDcIa7QpGw8dw9.QX1EDO0wCMyAzNzEzW}
i use man command and then did ?flag to find the correct argument to get me the flag 

### What i learned 
how i can scroll man pages with the arrow keys (and PgUp/PgDn) and search with / and can hit n to go to the next result and N to go to the previous result and use ? to search backwards!

# Searching For Manuals 

**FLAG:** pwn.college{owQtAAzTyFB168K5uknpPjgTLPv.QX2EDO0wCMyAzNzEzW}
i first used man man command to understand more about manpage. i went through the contents to find theres a -K (--global-apropos) command that could help me search the contents of all the manpages to find a particular keyword so i i tried man -K /challenge/challenge to find the hidden manpage and the argument --owtzyu NUM and that NUM is 168 so i typed that to obtain the flag

### What i learned 
how i use man man command to learn more about the man command and how man -K "keyword" searches all the manpages for the keyword

# Helpful Programs 

**FLAG:** pwn.college{Ypc7uauHKf8_oEWgyUnSdh2luF8.QX3IDO0wCMyAzNzEzW}
i first used /challenge/challenge --help to get details about different arguments i can use it with. so i tried all those different arguments but when i did /challenge/challenge -p i got a secret value 782 then i when i tried /challenge/challenge -g GIVE_THE_FLAG but i was not getting it then i realised i have to give the correct value so i used /challenge/challenge -g 782 and found the flag 

### What i learned 
how we can use --help to tell us how to run some commands which dont have manpage

# Help for Builtins 

**FLAG:** pwn.college{kuUVhFCudqoEYWWPQ-zzRDEVn3F.QX0ETO0wCMyAzNzEzW}
i tried help challenge and found that if i do challenge --secret SECRET with the correct secret value i will get the flag that this value is kuUVhFCu so i got the flag

### What i learned 
how we can use help with a particular command to look help for built-ins
