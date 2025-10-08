# DESCRIPTION 
As you step into the second chamber, 
a figure manifests before you. Before you stands a forgotten deity, a dead god spoken of only in whispers.
Known by countless names: “Apostle of Epilogue and Eternity,” “Lone Messiah” and many more lost to time.
They leave nothing but a single image, a relic carrying his final secret. Hidden within its layers lies 
the key to ascend to the next chamber.

![challenge](https://github.com/user-attachments/assets/7e8aa81d-a3c8-42f1-b78f-a89c855dea36)

# WRITE UP 

**FLAG:** citadel{th1s_ch4ll3ng3_1s_f0r_th4t_0n3_ex1ft00l_4nd_b1nw4lk_enthus14st}
we first exracted the meta data of the image using https://www.metadata2go.com/view-metadata which gave us the .json file which had the pixel details. which when observed further we found that there was a next marker FF E1 indicates the presence of an APP1 segment, commonly used for storing metadata like EXIF or XMP.

so we used https://www.unroll.ing/ to obtain the bin file of the data and then converted it to png using https://anyconv.com/bin-to-png-converter/#:~:text=Follow%20these%20simple%20steps%20to%20convert%20BIN%20files,%E2%80%9CConvert%E2%80%9D%20button%20to%20turn%20your%20BIN%20into%20PNG. to finally obtain the hidden image and the flag 

<img width="640" height="613" alt="AnyConv com__extracted_1759906756128" src="https://github.com/user-attachments/assets/c94be7fb-1729-4356-a32d-ee37ee0b2a06" />


