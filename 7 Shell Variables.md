#  Printing Variables

**FLAG:** pwn.college.{Udx86T_TPR6P0eBeFWEfnoFDfoL.QX3UTN0wCMyAzNzEzW}
i used echo $FLAG to obtain the flag

### What i learned 
how we can print out variables using echo $variablename

# Setting Variables

**FLAG:** pwn.college{80I8XKACL77BXtugpXQbJ50yQcE.QX5UTN0wCMyAzNzEzW}
i used PWN=COLLEGE to obtain the flag

### What i learned 
how we can feed values to a variable by using variable=value WITHOUT ANY SPACES!!!!!!

# Multi-Word Variables

 **FLAG:** pwn.college{MXEMF_wxCeO_xtbNMUbxsK55xkp.QXwYTN0wCMyAzNzEzW}
 i used PWN="COLLEGE YEAH" to obtain the flag

 ### What i learned 
how when there are more than 1 word to be fed into a variable we can use variable="two words"

# Exporting Variables

**FLAG:** pwn.college{09s6ffzJW3CRQSz0uMEc9RQx0wM.QXyYTN0wCMyAzNzEzW}
i first set COLLEGE to PWN variable and then set PWN to COLLEGE variable. then i exported PWN variable and then ran the command /challenge/run PWN 

### What i learned 
how variables that we set in a shell session are local to that shell process and other commands wont inherit them but we can do it by running the command export variable name 

# Printing Exported Variables 

**FLAG:** pwn.college{EWHOnu39w_lyRP_dJB5H1hNAe8d.QX4UTN0wCMyAzNzEzW}
i used to command env to obtain the flag

### What i learned 
how using env command we can print all the exported variables

# Storing Command Output

**FLAG:** pwn.college{ogDrQrVCywtcwg3TXJU8pDqf95e.QX1cDN1wCMyAzNzEzW}
i used PWN=$ `challenge/run /flag` to obtain the flag

### What i learned 
how we can store the output of some command into a variable by using variable name=$ (command /file)





