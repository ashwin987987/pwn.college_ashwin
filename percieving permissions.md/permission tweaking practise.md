# Challenge Name
permission tweaking practise

## My solve
**Flag:** `pwn.college{01NJPHgDOO16GAxwszQG7Nf0G8H.QXwEjN0wyN0gjNzEzW}`

```bash
Connected!
hacker@permissions~permission-tweaking-practice:~$ /challenge/run
Round 1 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod u+x,g+wx /challenge/pwn
You set the correct permissions!
Round 2 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod o+w /challenge/pwn
You set the correct permissions!
Round 3 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod o-rw /challenge/pwn
You set the correct permissions!
Round 4 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod u-w /challenge/pwn
You set the correct permissions!
Round 5 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod u+w,o+wx /challenge/pwn
You set the correct permissions!
Round 6 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod o-w /challenge/pwn
You set the correct permissions!
Round 7 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod o+rw /challenge/pwn
You set the correct permissions!
Round 8 of 8!
hacker@permissions~permission-tweaking-practice:~$ chmod o-r /challenge/pwn
You set the correct permissions!
You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!
hacker@permissions~permission-tweaking-practice:~$ chmod u+r /flag
hacker@permissions~permission-tweaking-practice:~$ cat /flag
pwn.college{01NJPHgDOO16GAxwszQG7Nf0G8H.QXwEjN0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to tweak permissions using u,g,o and +- terms in the chmod command

## References 
None
