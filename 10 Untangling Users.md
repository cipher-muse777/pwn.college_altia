# Becoming Root With Su 

**FLAG:** pwn.college{kipYHNrBT3EkMer89ht6ovdZFHr.QX1UDN1wCMyAzNzEzW}
first i used the su command and then entered the password to become root then i used cat /flag to obtain the flag

### What i learned
we can become the root by usind the su command and entereing the passowrd correctly

# Other Users With Su 

**FLAG:** pwn.college{8ChxfAxWzS6u3EIAedqqM99zzL_.QX2UDN1wCMyAzNzEzW}
i used the command su zardus and entered the password to switch the user then ran /challenge/run to obtain the flag 

### What i learned 
how we can switch users by running the command su user-name and entering the correct password

# Cracking Passwords 

**FLAG:** pwn.college{4bojoHGx_bXTPErdSshffxXbun5.QX3UDN1wCMyAzNzEzW}
i first ran the command john /challenge/shadow-leak then i did the command john --show /challenge/shadow-leak and obtained the password. then i did su zardus and entered the password to switch users. then i ran /challenge/run to obtain the flag 

### What i learned 
we can use john command to crack passwords on a leak /etc/shadow 

# Using Sudo 

**FLAG:** pwn.college{kWbkDfyIiUuS4I11W9AYLd25Brs.QX4UDN1wCMyAzNzEzW}
i used sudo cat /flag to obtain the flag

### What i learned 
how sudo command defaults to running a command as a root based on policies
