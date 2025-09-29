# Challenge Name
Intro to arguments

## My solve
**Flag:** `pwn.college{gBl2ymnD8G2_C93Kwj81xpbVx7V.01MzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!  (terminal 1)
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{gBl2ymnD8G2_C93Kwj81xpbVx7V.01MzMDOxwyN0gjNzEzW}  (terminal 2)
```
## Incorrect tangents I went on
I didnt open seperate  terminals to redirect it and cat it in y first attempt

## What I learned
I learned how to create FIFO files using mkfifo command and apply their properties

## References 
None
