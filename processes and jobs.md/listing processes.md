# Challenge Name
listing processes

## My solve
**Flag:** `pwn.college{cUf5CU6VLohFxuZR-7Ntr8Z_wbQ.QX4MDO0wyN0gjNzEzW}`

```bash
Connected!
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 15:06 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 15:06 ?        00:00:00 /run/dojo/bin/sleep 6h
root         132       1  0 15:06 ?        00:00:00 /challenge/2-run-7961
root         135     132  0 15:06 ?        00:00:00 sleep 6h
hacker       137       0  0 15:06 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       143     137  0 15:06 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       152       0  0 15:06 pts/1    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       158     152  0 15:06 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       169     158  0 15:07 pts/1    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/2-run-7961
Yahaha, you found me! Here is your flag:
pwn.college{cUf5CU6VLohFxuZR-7Ntr8Z_wbQ.QX4MDO0wyN0gjNzEzW}
Now I will sleep for a while (so that you could find me with 'ps').
```
## Incorrect tangents I went on
None

## What I learned
I learned to list processes using ps -ef or ps - aux command

## References 
None
