# DESCRIPTION

Your quest continues, but you feel something odd about this room. The only artifact on 
this floor is a corrupted file held in the hands of a jet-black statue, frozen in the pose of 
a band mid-performance. The passcode to the next floor is hidden within this piece of music, but 
it can’t be played, as if the wrong extension has scrambled it.
You must take the corrupted file and repair it to reveal the true code that will unlock the door forward.

# WRITE UP 
**FLAG:** citadel{8lackM1D1wa5c00l}
we get a .wav file which is cannot play as it is corrupted (the extension is wrong, 
it should be a midi file as hinted by description mid)Using hex editor, we change the
file extention to midi file (change header to MThd) opening the changed midi file in a 
music editor, we can see the keys played in it. The key pattern on screen shows us the flag.
https://private-user-images.githubusercontent.com/230803596/498904847-68f70469-dcb5-479f-a816-581b51483115.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5Mzc0NzEsIm5iZiI6MTc1OTkzNzE3MSwicGF0aCI6Ii8yMzA4MDM1OTYvNDk4OTA0ODQ3LTY4ZjcwNDY5LWRjYjUtNDc5Zi1hODE2LTU4MWI1MTQ4MzExNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNTI2MTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1iNzc0ZGZhYmQ4ZGI0NDVlYzFlOGFmZDQxOTZhZjQ2ODRjYWJiMjNhOGRlYmY2MGJmODI5NTcyNWI4NzI2NmVlJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.--0mTrj25nrW2UfXXNbWyPIpddHHAv61UGGFquaTRx4
