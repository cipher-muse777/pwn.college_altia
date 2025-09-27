# Redirecting Output 

**FLAG:** pwn.college{EmVjMqjmPxf3o3vcbFVn_pGxg0z.QX0YTN0wCMyAzNzEzW}
i used echo PWN>COLLEGE to redirect the output of echo PWN (ie is PWN) to COLLEGE file so i obtained the flag

### What i learned 
how we can use > to put a particular output to a file

# Redirecting More Output 

**FLAG:** pwn.college{ItNl1CBk-sPvI9nFC2ydMrezdYD.QX1YTN0wCMyAzNzEzW}
i saved the output of /challenge/run to myflag file using /challenge/run>myflag and then ran cat myflag to obtain the flag 

### What i learned 
how >  redirects the output of any command

# Appending Output 

**FLAG:** pwn.college{Ag7cGxFpYMeKHni3YEAI22oJaO7.QX3ATO0wCMyAzNzEzW}
i first ran /challenge/run>/home/hacker/the-flag and then ran /challenge/run>>/home/hacker/the-flag to redirect the two halves of the flag and then used cat /home/hacker/the-flag to obtain the flag

### What i learned 
> will create a new output file every time, deleting the old contents. so using >> will keep on adding to the same file without deleting old files

# Redirecting Errors

**FLAG:** pwn.college{sdXI6y6F275ZdzRUtcktCNF7Pq_.QX3YTN0wCMyAzNzEzW}
i first used /challenge/run>myflag 2>instructions and then ran cat myflag to obtain the flag

### What i learned 
A File Descriptor (FD) is a number that describes a communication channel in Linux. there are three of them FD 0 (input), FD 1 (output), FD 2 (error) and how not mentioning this number naturaly implies 1. using 2 enables to run command that might produce data via standard error

# Redirecting Input 

**FLAG:** pwn.college{ksnd9S_TtPmNovoYe2VfhWWFUU3.QXwcTN0wCMyAzNzEzW}
i first did echo COLLEGE>PWN to save COLLEGE to PWN and then i did /challenge/run < PWN which fed the conetnts of PWN to the command

### What i learned 
we can use command < file name to feed the values in the file to that particular command 


