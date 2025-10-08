# DESCRIPTION 
You come across the remnants of a fallen corporation and the final network communication ever sent by them.
Allegedly, the message contained an image that predicted the rise of the Citadel. Your task is to uncover what 
was sent and decode the communication to extract the passcode that will unlock the next floor.

# WRITE UP
**FLAG:** citadel{1_r34lly_w4nt_t0_st4y_4t_y0ur_h0us3}
the given .pcap file (thus we can see the network traffic)
it was observed that the ICMP (error detecting) has 2 packets. We searched for image file 
in it (Since description hinted at image) (could not find image file in TCP) and we found 
one jpg header in the 1st and 2nd ICMP packet We extracted the image bytes using 
CLI tshark -r challenge.pcap -Y "icmp" -w icmp_packets.pcap and visualised it in a Hex editor.
