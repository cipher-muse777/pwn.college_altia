# DESCRIPTION

The guardian of this floor steps from the shadows. Known only as Jack the Ripper,
he watches you carefully. He proclaims himself merciful and hands you a word list to help. 
He asks you to find the passcode hidden in the file. The word list is your only aid. 
Only by combining the two correctly, can you uncover the key and move on to the next floor

# WRITE UP
**FLAG:** citadel{fake_flag_4_fake_pl4y3rs}
We have a file and given a wordlist. We need to combine two of them to form the actual flag
the file with $2a$04$RNoyoWAcW0StwSri4YN1Eeb2j1gBNKutDOMxsLzfyfSvB/ghMHToa to be decoded
We decrypted the code in a hash identifier to come to bcrypt $2$, Blowfish (Unix)* as algorithm
To get password from wordlist.txt, we use john command (learnt in pwn.college). This gets us the 
password as fake_flag_4_fake_pl4y3rs
