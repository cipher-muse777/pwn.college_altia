# DESCRIPTION 
The door to the next floor is guarded by a figure who calls herself "The Dragon CEO". 
She does not speak of mercy or choice, only of order and efficiency.To enter the next 
chamber, you must complete the task presented by her. Complete it
exactly as instructed, achieving operational efficiency by her standards,
and the path forward will open.

Connection: nc chall_citadel.cryptonitemit.in 61234

# WRITE UP 
**FLAG:** citadel{k1ryu_c0c0_h4s_4_g0_4t_4n_uns0lv3d_m4th3m4t1cs_pr0bl3m}
We need to solve the problem statement in given pdf file:///C:/Users/Rochelle/Downloads/Coco_Conjecture.pdf 
We are given a network challenge where the server sends us random positive integers (1 ≤ n ≤ 10^18).
Our task is to compute how many steps it takes to reduce n to 1 using the following rules:

If n is even, replace n with n / 2.
If n is odd, replace n with 3n + 1 collatz conjecture
In the netcat, the server sends numbers line-by-line (each followed by a newline). 
For each number n we apply the Collatz transformation until it becomes 1 and count the number of steps.
when all numbers are answered correctly, the flag we obtaub the flag.

we use python code to automate this

```
from pwn import *

# Connect to the challenge
conn = remote('chall_citadel.cryptonitemit.in', 61234)

def steps(n):
   count = 0
   while n != 1:
       if n % 2 == 0:
           n //= 2
       else:
           n = 3 * n + 1
       count += 1
   return count

while True:
   data = conn.recvline().decode().strip()
   if not data:
       break
   if data.startswith("citadel"):
       print(data)
       break
   n = int(data)
   ans = steps(n)
   conn.sendline(str(ans))
```

