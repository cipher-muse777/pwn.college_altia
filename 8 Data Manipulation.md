# Translating Characters 

**FLAG:** pwn.college{Idjnl7GIpkEx9Ygr8nnEk1T5VuA.01MxEzNxwCMyAzNzEzW}
i used the command  /challenge/run | tr '[A-Z][a-z]' '[a-z][A-Z]' to case swap and obtain the flag

### What i learned 
how we can use | tr command to change a given letter in output of previous command ie, some command | tr A B and how to case swap we can use '[A-Z] '[a-z]' 

### References 
https://linuxopsys.com/convert-to-uppercase-or-lowercase-on-linux

# Deleting Characters 

**FLAG:** pwn.college{QG3yjh2C2gQyQ6igx2xZO2Hk4XN.0FNxEzNxwCMyAzNzEzW}
i used the command /challenge/run | tr -d '[% ^]' to delete and obtain the flag

### What i learned 
how we can delete characters we can use tr -d command ie, some command | tr -d A

# Deleting Newlines 

**FLAG:** pwn.college{0aMJb0TJT0bdzjiygYlqlOp7pme.0VNxEzNxwCMyAzNzEzW}
i used the command /challenge/run | tr -d "\n" to delete the newlines and obtain the flag

### What i learned 
how we can specify newlines using the, some command | tr _ "/n" this causes the second word of the output to start in the next line 

#   Extracting The First Lines With Head 

**FLAG:** pwn.college{EuN3_NwCnOJ9w3s15FnBrO6mf02.0lNxEzNxwCMyAzNzEzW}
i used the command /challenge/pwn | head -n 7 | /challenge/college to obtain just the first 7 lines of the output of /challenge/pwn and then i pipied into /challenge/college to obtain the flag

### What i learned 
how we can specify a particular number of lines out of a very long output of a cmmand by using command | head -n some number

# Extracting Specific Sections Of Section 

**FLAG:** pwn.college{M4B_NssAYnnyQoq86oabzBpngvp.01NxEzNxwCMyAzNzEzW}
i used the command /challenge/run |cut -d " " -f 2 | tr -d "\n" to grab 2nd columns of data and then deleted all the newlines

### What i learned 
we can extract specific columns of a data by using some command | cut -d " " -f coloumn-no

# Sorting Data 

**FLAG:** pwn.college{s-Njdy4SYQTuqSDqU3fx5yIuA4V.0FM0MDOxwCMyAzNzEzW}
i used the command sort /challenge/flags.txt alphabetically and obtained the flag 

### What i learned 
how we can sort throught a file using sort command. by defaults is alphabetical and then we can use arguments like -r (reverse order) -n (for numbers) -u (remove duplicates) -R (random order)


