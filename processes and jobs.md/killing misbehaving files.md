# Challenge Name
killing misbehaving files
## My solve
**Flag:** `pwn.college{oao6qL3_PYR8ZHkw2AMw1RWdoGv.0FNzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@processes~killing-misbehaving-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 05:44 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 05:44 ?        00:00:00 /run/dojo/bin/sleep 6h
root         137       1  0 05:44 ?        00:00:00 /bin/bash /challenge/.init
root         138       1  0 05:44 ?        00:00:00 /bin/bash /challenge/.init
root         139       1  0 05:44 ?        00:00:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         140     137  0 05:44 ?        00:00:00 sleep 6h
root         141     138  0 05:44 ?        00:00:00 sleep 6h
hacker       142     139  0 05:44 ?        00:00:00 /usr/bin/python /challenge/decoy
hacker       144       0  0 05:45 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       150     144  0 05:45 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       159     150  0 05:45 pts/0    00:00:00 ps -ef
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!   (terminal 1)
hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{oao6qL3_PYR8ZHkw2AMw1RWdoGv.0FNzMDOxwyN0gjNzEzW}      (terminal 2)
```
## Incorrect tangents I went on
None

## What I learned
I learned to kill processes by using kill command by listing them using ps -ef

## References 
None
