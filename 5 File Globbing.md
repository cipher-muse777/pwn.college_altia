# Matching with *

**FLAG:** pwn.college{wapbGcCOfrBtc7z-dKKe6QHwMSh.QXxIDO0wCMyAzNzEzW}
i first opened /challenge wusing cd /ch* since there was a restirction of maximum 4 characters then i ran /challenge/run using /c*/r* so obtain the flag

### What i learned 
the * causes the shell to replace the argument with any possible files that match the pattern 

# Matching with ?

**FLAG:** pwn.college{w9fC2fLOtvW-XxM1F5NdyBy8wmf.QXyIDO0wCMyAzNzEzW}
 i opened /challenge using cd /?ha??enge and then ran /challenge/run using /?ha??enge/run to obtain the flag 

 ### What i learned 
 the ? causes the shell to replace the argument with single character wildcard

 # Matching with []

 **FLAG:** pwn.college{4vIC821awGWz2uH7ab9zP68tWtI.QXzIDO0wCMyAzNzEzW}
 i first opened /challenge/files and then ran /challenge/run file_[bash] to obtain the flag

 ### What i learned 
 the [] is like the limited form of ? which is a wildcard for some subset of potential characters, specified within the brackets

 # Matching paths with [] 

 **FLAG:** pwn.college{QaqzY9rdORPvHPcgD7VOM7-zqtm.QX0IDO0wCMyAzNzEzW}
 i initially for an unholy amount of time used /challenge/run /home/hacker/challenge/files/file_[bash] and didnt get the flag to my further frustration and then realised the /home/hacker was absolutely unecessary so instead i used /challenge/run /challenge/files/file_[bash] to obtain the flag

 ### What i learned 
 how we can expland paths using [] globs 
 
# Multiples Globs 

**FLAG:** pwn.college{IrCpdZ3ku26TbWaRDNvvAwlroVm.0lM3kjNxwCMyAzNzEzW}
i first opened /challenge/files using cd and then used /challenge/run * p * (without the spaces) to find all the files that had a p in its name

### What i learned 
how we can use two globs and to find all the files with the letter enclosed inside the globs 

# Mixing Globs 

**FLAG:** pwn.college{sI2-6PqEvaBfTf9Bahxpn9csgfF.QX1IDO0wCMyAzNzEzW}
i first opened /challenge/files using cd command then tried using /challenge/run * [li] * which gave me words with l or i inside the word /challenge/run * [ing] it gave me words that ends in ing and then finally used /challenge/run [cep] * which gave me words that start with c e and p the finally gave me the flag 


### What i learned 
how we can mix globs to search and obtain files paths etc like we need 

# Exclusionary Globbing

**FLAG:** pwn.college{MmutoNdXXtIHHldntD0YscaReHT.QX2IDO0wCMyAzNzEzW}
i first opened /challenge/files using cd and then used /challenge/run [!pwn]* to exclude words that start with p w n

### What i learned 
how we can exclude words by using [!word] or [^word] 

# Tab completeion 

**FLAG:** pwn.college{gCj-EO9GztI2xaxiJCBZvnFpfKx.0FN0EzNxwCMyAzNzEzW}
i used /challenge/pwn then clicked the tab button to finish the command and then obtained the file 

### What i learned 
how sometimes * globbing might cause errors so using tab button will auto-complete it

# Multiple Options For Tab Completeion 

**FLAG:** pwn.college{4L0Kxdul8FBChuTQdIKzuShHAyI.0lN0EzNxwCMyAzNzEzW}
i used /challenge/files/p and then tab button to see all possible files and then started reading them one by one using cat and tab till i read /challenge/files/pwncollege-flag from which i got the flag

### What i learned 
when there are multiple options we can use the tab button to see all possible outcomes and then manually manueuver through it 

# Tab Completion On Commands 

**FLAG:** pwn.college{sAT5__M6UZ8Tpwq3X0fpBCDBNyf.0VN0EzNxwCMyAzNzEzW}
i typed pwncollege then hit tab button which auto-completed it into pwncollege-3455 

### What i learned 
we can auto-complete commands too but we need to double check before running them 
