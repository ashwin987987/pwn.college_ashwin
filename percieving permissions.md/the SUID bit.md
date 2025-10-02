# Challenge Name
the SUID bit

## My solve
**Flag:** `pwn.college{IdCXr_GIPIoOCnh1zWJq5X6cpA-.QXzEjN0wyN0gjNzEzW}`

```bash
Connected!
hacker@permissions~the-suid-bit:~$  chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{IdCXr_GIPIoOCnh1zWJq5X6cpA-.QXzEjN0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learnt to get the suid access to a file using u+s 

## References 
None
