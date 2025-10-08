# DESCRIPTION

You step into a simulation of the past, entering the ruins of AetherCorp, the most ambitious corporation in 
history, and their creation, NetProbeX, once the most advanced networking tool the world had ever seen. The 
floor reconstructs the events that led to humanity’s downfall. Your task is to find the hidden backdoor in NetProbeX, 
the flaw that triggered the collapse. By uncovering it, you can reverse the damage and retrieve the passcode to 
advance to the next floor. Engineers left faint traces in the logs — small, odd markers where separators once sat. 
Read these traces as if they divide commands.

Challenge: http://chall_citadel.cryptonitemit.in:32772/

# WRITE UP 
**FLAG:** citadel{17_1s_jus7_7h3_b3g1nn1ng}
https://private-user-images.githubusercontent.com/230803596/498903072-bd27f775-bf3b-4348-bd58-060607fbdc9a.JPG?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5Mzc0NzEsIm5iZiI6MTc1OTkzNzE3MSwicGF0aCI6Ii8yMzA4MDM1OTYvNDk4OTAzMDcyLWJkMjdmNzc1LWJmM2ItNDM0OC1iZDU4LTA2MDYwN2ZiZGM5YS5KUEc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNTI2MTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT04MmNjZDYxMGY2MDQzMmVlOTg2N2QxN2UzMzkyYWNiYmQyYTg3ODIwOWI3MmQ4MzA0OTI4ZmFmNDJjOWE4ZGRlJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.CvADBaLsHVVY2co_zB2kjuYgY_Fgd9PpfxQVDn4SKjA
After trying various pings, we realise that many separators (like . , ; {} etc) are malicious
%0A is being accepted, so we use it to enter commands and the ls command helps list out all files, 
out of which one is mission_briefing.txt, we use less (since cat is not allowed) to read the file Agent, 
your objective is to recover the Blacksite Key. Our intel confirms it’s hidden deep within the AetherCorp network
We find the aerthercorp directory and list its files (using ls AND ls -a to find secret files)
We get .secrets directory and get blacksite_key.dat file, reading which we get the flag.
