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

 **FLAG:** 
 
