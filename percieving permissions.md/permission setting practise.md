# Challenge Name
permission setting practise

## My solve
**Flag:** `pwn.college{kaJ9PrSL0oz4AeYjTeXdtVC2-46.QXzETO0wyN0gjNzEzW}`

```bash
Connected!
hacker@permissions~permissions-setting-practice:~$ /challenge/run
Round 1 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=x,g=rwx,o=w /challenge/pwn
You set the correct permissions!
Round 2 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=wx,g=r,o=x /challenge/pwn
You set the correct permissions!
Round 3 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=x,g=,o=rw /challenge/pwn
You set the correct permissions!
Round 4 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=x,g=rw,o=rwx /challenge/pwn
You set the correct permissions!
Round 5 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=rx,g=rwx,o=r /challenge/pwn
You set the correct permissions!
Round 6 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=rwx,g=rx,o=r /challenge/pwn
You set the correct permissions!
Round 7 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=,g=rwx,o=rwx /challenge/pwn
You set the correct permissions!
Round 8 of 8!
hacker@permissions~permissions-setting-practice:~$ chmod u=wx,g=,o=rx /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!
hacker@permissions~permissions-setting-practice:~$ chmod u=r /flag
hacker@permissions~permissions-setting-practice:~$ cat /flag
pwn.college{kaJ9PrSL0oz4AeYjTeXdtVC2-46.QXzETO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about arguments

## References 
None
