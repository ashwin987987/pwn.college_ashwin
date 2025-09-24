# Challenge Name
listing files

## My solve
**Flag:** pwn.college{U30zAzCj5BqLezbfoHRgt0r0tJa.QX4IDO0wyN0gjNzEzW}

```bash
Connected!
hacker@commands~listing-files:~$ 1s /challenge
bash: 1s: command not found
hacker@commands~listing-files:~$ 1s /challenge
bash: 1s: command not found
hacker@commands~listing-files:~$ ls /challenge
19980-renamed-run-11397  DESCRIPTION.md
hacker@commands~listing-files:~$ description.md
bash: description.md: command not found
hacker@commands~listing-files:~$ 19980-renamed-run-11397
bash: 19980-renamed-run-11397: command not found
hacker@commands~listing-files:~$ /19980-renamed-run-11397
bash: /19980-renamed-run-11397: No such file or directory
hacker@commands~listing-files:~$ /challenge/19980-renamed-run-11397
Yahaha, you found me! Here is your flag:
pwn.college{U30zAzCj5BqLezbfoHRgt0r0tJa.QX4IDO0wyN0gjNzEzW}
```
## Incorrect tangents I went 
i didnt give the right path for the renamed file twice and i used 1s instead of ls twice

## What I learned
I learned about ls command to list all the files in a directory

## References 
None
