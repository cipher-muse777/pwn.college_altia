# DESCRIPTION

This floor is haunted by a phantom of the past. You encounter a presentation created by the last employee 
of a forgotten corporation, made just minutes before the Citadel awoke. Rumor has it that the corporation 
predicted the rise of the Citadel. Within the slides, a "starter pack" holds the clues you need. Use it to
confront the "final boss," a threat trapped inside a macro hidden deep within the presentation, and 
claim the key to the next floor

# WRITE UP 
**FLAG:** citadel{gr4b_y0ur_l4bubus_m4tch4s_4nd_dub41_ch0c0l4t3s_y0u_4r3_1n_f0r_4_r1d3}
We are given a .pptm file instructing us to use macro. So we enable the developer tab and view the VBA (Visual Basic) code 
There are three parts to the code. The first part is Base32 encoded, second is base64 and third 
is base32. Each part is further divided into many strings. Concatenating all of the string parts and 
decoding them gets us the bytes of a JPG file (image, as seen by the header FF D8 FF E0) 
Each part of the code is a part of the image forming

https://private-user-images.githubusercontent.com/230803596/498903938-877c55ec-47b0-443b-b28b-e7982275aa5a.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5Mzc0NzEsIm5iZiI6MTc1OTkzNzE3MSwicGF0aCI6Ii8yMzA4MDM1OTYvNDk4OTAzOTM4LTg3N2M1NWVjLTQ3YjAtNDQzYi1iMjhiLWU3OTgyMjc1YWE1YS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNTI2MTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0zYzUyMjcxNmY3OGEzOGRjZDVmZGRmNjJiOTBkNWI3MGE4NDI0ODA5NjUzMWJjMTNhYTg3MDE3YzM2ZWI1MWExJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.3_jwuA6kJhIMP0nIckFv_ZMqwX5MXbSAWaNBGajEh2E

