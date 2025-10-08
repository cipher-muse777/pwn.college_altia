# DESCRIPTION 

After finding the backdoor and making your way to the next floor, you step into a chamber awash 
with shifting colors and swirling echoes, a concert frozen in time. Kevin Parker stands at the 
center, his riffs bending reality around him. To ascend, you’ll need to join the session on his 
terms: push your voice further than comfort, align yourself with the number he hides in the haze, 
and piece together the melody concealed within layers
of reverb. Only then will the music open the way upward.

# WRITE UP 
**FLAG:** citadel{17_1s_jus7_7h3_b3g1nn1ng}
We get a code which we can use by reverse engineering it. We open it into ghidra (reverse engineering software) 
thus we can see that FUN_00101240 is the main function (has constants) 1340 and 14c0 are for level 2 and level 1 (redundant), 
thus main is 1240 flag is formed using the code, giving us the flag
