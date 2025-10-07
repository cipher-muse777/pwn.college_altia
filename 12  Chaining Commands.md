# Chaining With Semicolons 

**FLAG:** pwn.college{8T4ivH3Xx3hmOQ11-t8Gf2XbrPu.QX1UDO0wCMyAzNzEzW}
i executed /challenge/pwn; /challenge/college to obtain the flag

### What i learned 
how we can chain commands using ; where the first command is executed and then the second

# Building On Success 

**FLAG:** pwn.college{IlPwmrAjk4yruZyZTWGS_WsmHMs.0lM0MDOxwCMyAzNzEzW}
i executes /challenge/first-success && /challenge/second to obtain the flag 

### What i learned 
how we can use the AND operator (&&) that executes the second command only if the first is successful 

# Handling Failure 

**FLAG:** pwn.college{QFeWxxjtQNeH_2nwUIKDYho92di.01M0MDOxwCMyAzNzEzW}
i executed /challenge/first-failure || /challenge/second to obtain the flag

### What i learned 
how we can use the OR operator (||) that executes the second command only if the first is a failure 

# Your First Shell Script 

**FLAG:** pwn.college{
