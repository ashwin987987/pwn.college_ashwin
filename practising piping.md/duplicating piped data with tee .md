# Challenge Name
duplicating piped data with tee

## My solve
**Flag:** `pwn.college{g1JVxy-b6emw8Y9BQZMIM7QgauU.QXxITO0wyN0gjNzEzW}`

```bash
Connected!
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pwn | /challenge/college
Processing...
WARNING: you are overwriting file pwn with tee's output...
catThe input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "g1JVxy-b"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret g1JVxy-b
Processing...
You must pipe the output of /challenge/pwn into /challenge/college (or 'tee'
for debugging).
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret g1JVxy-b | tee pwn | /challenge/college
Processing...
WARNING: you are overwriting file pwn with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{g1JVxy-b6emw8Y9BQZMIM7QgauU.QXxITO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
I initially used the wrong order of commands

## What I learned
I learned about to duplicate piped data using tee command to see what passes through while piping one file to another ( debugging)

## References 
None
