# The PATH Variable 

**FLAG:** pwn.college{gh0bwzRuxp-LqBoIyS7OqVuxf5A.QX2cDM1wCMyAzNzEzW}
i executed PATH="" to make sure /challenge/run cannot find the rm command to delete the flag and the executed /challenge/run to obtain the flag

### What i learned 
how PATH is a special shell variable that stores a bunch of directory paths in which the shell will search for programs corresponding to commands and leaving is blank PATH="" causes bash unable to find commands

# Setiing PATH

**FLAG:** pwn.college{EoQStAMrj5NMTQOfnsfANy3Cs2o.QX1cjM1wCMyAzNzEzW}
i first executed PATH=/challenge/more_commands to overwrite the PATH and then ran the command /challenge/run

### What i learned 
how we can use PATH to add directories to the list so a program can be launched without having to mention its whole path every time

# Finding Commands

**FLAG:** pwn.college{ojje87WPOw_mSLSxeDi3Bja2trx.01NzEzNxwCMyAzNzEzW}
i first executed which win and showed me the directory it was placed in so i used cat /challenge/paths/17727/flag to obtain the flag

### What i learned 
how we can use which command that the looks at each directory in $PATH in order and prints the first file it finds whose name matches the argument you passed.

# Adding Commands 

**FLAG:** pwn.college{YbiSlBM6a_R21v4bdxYG8OW7DYD.QX2cjM1wCMyAzNzEzW}
i first created a directory using mkdir /tmp/pwn then i opened it using cd command and then i did echo "/bin/cat /flag" > win and then executed chmod +x win AND FINALLY PATH="/tmp/pwn/:$PATH" /challenge/run to obtain the flag

### What i learned 
how we can add a new directory to a path rather than wiping and redefining it every time by using PATH="/new/directory:$PATH"

# Hijacking Commands

**FLAG:** pwn.college{0Xy2LTJnWLo0wgDt3gOCbnnz3Go.QX3cjM1wCMyAzNzEzW}
i first created a directory using mkdir /tmp/pwn then i echo '#!/bin/bash' > /tmp/pwn/rm to make a fake command script with shebang and then used chmod a+x /tmp/pwn/rm to give permissions 
PATH="/tmp/pwn:$PATH" THEN FINALLY ran /challenge/run to obtain the flag
