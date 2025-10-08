# DESCRIPTION 
You enter a virtual maze, a labyrinth of shifting corridors and endless paths. 
A guardian robot patrols the floor, leaving a trail behind as it moves. Follow 
the path it carves, trace its movements carefully, and uncover the key it leads you to. 
Only by following the robot’s trail can you reach the door to the next floor. 
Challenge: https://therobotstrail.citadel.cryptonitemit.in

# WRITE UP 
**FLAG:** citadel{p4th_tr4v3rs4l_m4st3ry_4ch13v3d}
the website opens to 5 decoy buttons, out of which none are correct. We use inspect to find the hidden hint
alt text On hidden class, we get hint to search /robots.txt alt text From here, we get hint 
<img width="1214" height="368" alt="image" src="https://github.com/user-attachments/assets/a1ce5e9f-3417-4b46-aa7b-8363b0825d86" />
file /etc/passwd tells us to check the web server config at /var/www/html/config.php:/home/webadmin:/bin/bash\n then we are asked 
to check the access logs for unusual activity and log has location /var/log/apache2/access.log
message Interesting environment variables might be found at /proc/self/environ is next hint SECRET_LOCATION=/home/ctf/.secret 
is our next hint then finally we get the flag at /home/ctf/.secret/flag.txt
