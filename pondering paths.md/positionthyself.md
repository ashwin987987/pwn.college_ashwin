 #Challenge Name
position thy self

## My solve
**Flag:** pwn.college{sP-M2GIGb5KrEZHTbk6S8i6elIA.QX2QTN0wyN0gjNzEzW}

```bash
Connected!
hacker@paths~position-thy-self:~$ cd /some/new/directory
bash: cd: /some/new/directory: No such file or directory
hacker@paths~position-thy-self:~$ cd /challenge/run
bash: cd: /challenge/run: Not a directory
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /tmp
hacker@paths~position-thy-self:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{sP-M2GIGb5KrEZHTbk6S8i6elIA.QX2QTN0wyN0gjNzEzW}
```
## Incorrect tangents 
instead of running the challenge run code i used cd on challege run and found out it was not the directory 

## What I learned
I learned about the change directory(cd command)

## References 
None
