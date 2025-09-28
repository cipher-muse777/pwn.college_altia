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

# Grepping Stored Results

**FLAG:** pwn.college{cuUMWhh5twqGtps018tBPjTRL5b.QX4EDO0wCMyAzNzEzW}
i first used /challenge/run > /tmp/data.txt to redirect the output of /challenge/run to /tmp/data.txt and then did grep flag /tmp/data.txt which gave me a list of words with the word flag so then i tried grep pwn.college /tmp/data.txt to obtain the flag 

### What i learned 
how using grep command helps us sort through thousands of lines of code 

# Grepping Live Output

**FLAG:** pwn.college{IgMexXQzlGg_0S4tSc1pbRdH5YM.QX5EDO0wCMyAzNzEzW}
i used the command  /challenge/run | grep pwn.college to obtain the flag

### What i learned
how we can avoid the need to store results to a file but using | command that helps us pipe the standard output of left to the standard input of right

# Grepping Errors

**FLAG:** pwn.college{gFZwKwjFkpRQxhIGzWvo3lc5qJd.QX1ATO0wCMyAzNzEzW}
i used /challenge/run 2>& 1| grep pwn.college to obtain the flag

### What i learned 
how we can grep through the errors directly by using command 2>&1 | another command

# Filtering With Grep-v 

**FLAG:** pwn.college{QmMGEkTr24Q3SEqKFYxp2rkBawI.0FOxEzNxwCMyAzNzEzW}
i used /challenge/run | grep -v DECOY to obtain the flag

### What i learned 
how we can sort through the files not having a particular word using grep -v word 

# Duplicating Piped Data With Tee

**FLAG:** pwn.college{QeqQRhxP8f7Nr8jOI4B2W1WigLY.QXxITO0wCMyAzNzEzW}
i first used /challenge/pwn | tee blehhh | /challenge/college to intercept the data i needed to use to pipe the contents from pwn to college. then i did cat blehhh and understood that i had to use /challenge/pwn --secret QeqQRhxP so after running /challenge/pwn |--secret QeqQRhxP /challenge/college i got the flag

### What i learned 
we can use tee to duplicate data flowing through your pipes to any number of files provided on the command line helping us to debug things

# Process Substitution For Input

**FLAG:** pwn.college{Qy_pIFulndWGwaTF7Qi6ZetvXw_.0lNwMDOxwCMyAzNzEzW}
i used diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag) and i got the flag

### What i learned 
how we can use <(command) to run the command and  hook up its output to a temporary file that it will create.

# Writing To Multiple Programs

**FLAG:** pwn.college{ALeFnATXRFMFACU4crW3DcESFIm.QXwgDN1wCMyAzNzEzW}
i used /challenge/the < <(/challenge/hack | tee >( /challenge/planet )) to send the outputs of /challenge/hack to both /challenge/the and /challenge/planet to obtain the flag

### What i learned 
how we can dupicate data into two files using tee and we can obtain desired commands using <() <<() etc etc

# Split-Piping Stderr and Stdout 

**FLAG:** pwn.college{AjFzEbV68SFxtqEo89S3Vm520kj.QXxQDM2wCMyAzNzEzW}
i used /challenge/hack 1> >(/challenge/planet) 2> >(/challenge/the) to duplicate the output of /challenge/hack to /challenge/planet and then send the error yo /challenge/the to obtain the flag


### What i learned 
we can use multiple pipings in one single line of code

# Named Pipes

**FLAG:** 
