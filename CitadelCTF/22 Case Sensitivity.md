#DESCRIPTION 

You step into a constricted floor where every movement and operation is limited. Commands are few, space is tight, 
and options are restricted. A guardian looms over the floor, its body shifting like liquid metal, enforcing these 
constraints. It watches your every move, daring you to make do with what you have and uncover the passcode to the 
next floor despite the restrictions.

Connection: nc chall_citadel.cryptonitemit.in 32770

# WRITE UP 
**FLAG:** 
We need to do the challenge in the given netcat
```
Ha, I bet you can't find what "FLAG" is in this shitty python interpreter.
 What could you possibly even do here?

>>>
```
Giving any word or command gives us error ValueError: NUH UH, cat is not allowed! When we give certain words like 
print or environ, it shows ValueError: NUH UH, environ is not allowed! (although environ is very close). This can 
be made right using captial letters as PRINT and ENVIRON (since challenge name is case sensitivity) which changes 
the error to NameError: name 'ENVIRON' is not defined Giving command exec is allowed. Using the whitelist words, we 
can find out the correct command to be exec("PRINT(ENVIRON".lower() + "['FLAG'])") which gives the flag

