# Chaining With Semicolons 

**FLAG:** pwn.college{8T4ivH3Xx3hmOQ11-t8Gf2XbrPu.QX1UDO0wCMyAzNzEzW}
i executed /challenge/pwn; /challenge/college to obtain the flag

### What i learned 
how we can chain commands using ; where the first command is executed and then the second

# Building On Success 

**FLAG:** pwn.college{IlPwmrAjk4yruZyZTWGS_WsmHMs.0lM0MDOxwCMyAzNzEzW}
i executed /challenge/first-success && /challenge/second to obtain the flag 

### What i learned 
how we can use the AND operator (&&) that executes the second command only if the first is successful 

# Handling Failure 

**FLAG:** pwn.college{QFeWxxjtQNeH_2nwUIKDYho92di.01M0MDOxwCMyAzNzEzW}
i executed /challenge/first-failure || /challenge/second to obtain the flag

### What i learned 
how we can use the OR operator (||) that executes the second command only if the first is a failure 

# Your First Shell Script 

**FLAG:** pwn.college{EvHO78Vr1sI46TvuoRbIaBnTb6H.QXxcDO0wCMyAzNzEzW}
i first executed touch x.sh then i did echo "/challenge/pwn; /challenge/college" > x.sh and then bash x.sh to obtain the flag

### What i learned 
how when the combined prompt gets super lengthy we can just feed it to a .sh file to make it easier by first creating it using touch command and then echoing our commands into .sh file and then running bash command.

# Redirecting Script Output

**FLAG:** pwn.college{gv2wa2E0GaQMMg2vklLKd-4FqlJ.QX4ETO0wCMyAzNzEzW}
i first created a .sh file using touch script.sh command and then i did echo "challenge/pwn; /challenge/college" > script.sh and then i used the pipe command to redirect the output into /challenge/solve by doing bash script.sh | /challenge/solve

### What i learned 
how we can redirect script files into other commands using bash .sh | other command

# Executable Shell Files

**FLAG:** pwn.college{ME2-4KIA22H_UoKQ_CXb_X3Vlc5.QX0cjM1wCMyAzNzEzW}
i first executed touch script.sh and then did echo "/challenge/solve" > script.sh and then changed the file permissions using chmod a+rwx script.sh and then ran ./script.sh to obtain the flag

### What i learned 
how we can make an executable script file by changing the permissions using chmod commandand then running it

# Understanding Shebangs

**FLAG:** pwn.college{4aJSjs5Ptnu5-HcYyU6DAGSSVl6.0VOzMDOxwCMyAzNzEzW}
i first executed cat > /home/hacker/solve.sh to make sure my file doesn't have a blank line initially and then i ran 
```
#!/bin/bash     
echo "hack the planet"
```
then ctrl+d to exit and then changed permissions using chmod a+x solve.sh and then executed /challenge/run to obtain the flag

### What i learned 
how we can use cat> filename to make create a new file and type content directly into it from the terminal. thereby helping us not have a blankline initially which will be there if we use touch command and how #!/bin/bash for bash scripts
#!/usr/bin/python3 for Python scripts #!/bin/sh for POSIX shell scripts helps Linux treat the file as an interpreted program, and the contents of the rest of the line as the path to the interpreter. It then invokes the interpreter with the path to the program file as its only argument.

### References 
https://www.geeksforgeeks.org/linux-unix/cat-command-in-linux-with-examples/

# Scripting With Arguments

**FLAG:** pwn.college{snsCnQkT67vXK8AQElM6SsGYvWJ.0VNzMDOxwCMyAzNzEzW}
i first executed cat> /home/hacker/solve.sh and then 
```
#!/bin/bash
echo $2 $1
```
then ctrl+d to exit i ran  bash /home/hacker/solve.sh pwn college to make sure i had the required outcome and then executed /challenge/run to obtain the flag

### What i learned
how we can use echo $1 $2 $3 etc to accept and decide the order of the arguments 

# Scripting Wuth Conditionals

**FLAG:** pwn.college{AM3v9s7vMaMH567QOscOgJL-htw.0lNzMDOxwCMyAzNzEzW}
i first executed cat> /home/hacker/solve.sh and then 
```
#!/bin/bash
if [ "$1" == "pwn" ]
then 
 echo "college" 
fi
```
and then bash /home/hacker/solve.sh pwn to make sure i had the required outcome and then executed /challenge/run to obtain the flag

### What i learned
how we can use if [ "$1" == "someword" ] to obtain a particular output if a particular argument is used with bash. DONT FORGET THE SPACES INSIDE THE SPACE.

# Scripting With Default Cases

**FLAG:** pwn.college{grexWd2Wyu9Pjdmx8DkQaCjQTTd.01NzMDOxwCMyAzNzEzW}
i first executed cat> /home/hacker/solve.sh and then 
```
#!/bin/bash
if [ "$1" == "pwn" ]
then 
 echo "college" 
else
 echo "nope"
fi
```
and then bash /home/hacker/solve.sh pwn to make sure i had the required outcome and then executed /challenge/run to obtain the flag

### What i learned 
how we can use if [ "$1" == "someword" ] along with else to obtain a particular output if a particular argument is used with bash 

# Scripting With Multiple Conditions

**FLAG:** pwn.college{4_IHzBYBzjJ-yoxAEBUbvXnk8xP.0FOzMDOxwCMyAzNzEzW}
i first executed cat> /home/hacker/solve.sh and then 
```
#!/bin/bash
if [ "$1" == "hack" ] 
then 
 echo "the planet" 
elif [ "$1" == "pwn" ]
then 
 echo "college"
elif [ "$1" == "learn" ]
then 
 echo "linux"
else 
 echo "unknown"
fi
```
and then bash /home/hacker/solve.sh pwn to make sure i had the required outcome and then executed /challenge/run to obtain the flag

### What i learned 
how we can use if [ "$1" == "someword" ] along with elseif [ "$1" == "something" ] and else to obtain a particular output and its various different possibilities if a particular argument is used with bash 

# Reading Shell Scripts 

**FLAG:** pwn.college{cwZIgS5YJubTj2Rb_kcUWeLdyZz.0lMwgDOxwCMyAzNzEzW}
i first executed cat /challenge/run to read the shell script which gave me the password that is hack the PLANET. then i ran /challenge/run and then entered the password to obtain the flag

### What i learned 
how we can use the cat command to read a shell script that requires you to put in a secret password, but that password is hardcoded into the script iself

