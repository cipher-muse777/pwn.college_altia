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
i first executed cat > /home/hacker/solve.sh to make sure my file doesn't have a blank line initially 
