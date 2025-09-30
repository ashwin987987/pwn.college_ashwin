# Challenge Name
suspending processes

## My solve
**Flag:** `pwn.college{8odmLfvHG8Vnm5AbIs-_Vj1xkLZ.QX1QDO0wyN0gjNzEzW}`

```bash
Connected!
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         169     140  0 16:31 pts/0    00:00:00 bash /challenge/run
root         171     169  0 16:31 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         169     140  0 16:31 pts/0    00:00:00 bash /challenge/run
root         176     140  0 16:31 pts/0    00:00:00 bash /challenge/run
root         178     176  0 16:31 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{8odmLfvHG8Vnm5AbIs-_Vj1xkLZ.QX1QDO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use ctrl+z to suspend the given process within the terminal

## References 
None
