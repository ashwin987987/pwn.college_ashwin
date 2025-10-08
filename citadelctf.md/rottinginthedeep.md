# writeup
Flag is converted to an integer and each digit is shifted by 3. Reversing the process gets the flag.

from Crypto.Util.number import *
ct = '6895840967002953721051398351211751734500850509315790892845302801984496338433523326225010635779036738800318'
flag = ''
for digit in ct:
    flag += str((int(digit)-3)%10)

print(long_to_bytes(int(flag)))
# flag: 
citadel{br0_r34lly_unr0tt3d_m3_b4ck_t0_l1f3}
