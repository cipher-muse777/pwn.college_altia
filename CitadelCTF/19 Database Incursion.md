# DESCRIPTION 

After your legendary battle with the artist, the virtual world has returned, stretching around you in 
endless grids and flickering data, you find a rogue data terminal and on careful inspection, you find you’re
able to inject rogue structured queries. Using this critical vulnerability, find a way to extract the hidden passcode.

Challenge: https://databaseincursion.citadel.cryptonitemit.in

# WRITE UP
**FLAG:** citadel{wh3n_w1ll_y0u_f1nd_0u7_1f_175_5ql_0r_53qu3l?}
https://private-user-images.githubusercontent.com/230803596/498903236-d140da0e-b947-4b59-9017-48b7a7dac503.JPG?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTk5Mzc0NzEsIm5iZiI6MTc1OTkzNzE3MSwicGF0aCI6Ii8yMzA4MDM1OTYvNDk4OTAzMjM2LWQxNDBkYTBlLWI5NDctNGI1OS05MDE3LTQ4YjdhN2RhYzUwMy5KUEc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUxMDA4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MTAwOFQxNTI2MTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wZjQwZGJkN2ZiZjIyZmUzOTIwMDY3NDQ1ZTMzNzAzYjUwMjE1N2U0Njg5ZjlkYWQ3NWMxMTcxYjQyMzEzNjkxJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.y02yVDQA9_gXzrepIVcNUIj1DdsJ_TRVFdvIinPIkaQ
to obtain the username and password We use SQLi. We input something in the working payload which is always true 
(in this case, we inputted 1=1 which is always true). From here, we come to a page where we have employee details 
(we need to enter admin password) Hint: someone from management has the admin password. We see the management people 
department='Management'-- and we see that KIWI has the password We search for kiwi from management (department='Management' 
and name='Kiwi')-- Thus we get the flag from the employee
