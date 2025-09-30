# Challenge Name
resuming processes

## My solve
**Flag:** `pwn.college{E8SOQCUl3k0pPqgJ6yO9OWpx9Kf.QX2QDO0wyN0gjNzEzW}`

```bash
Connected!
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg /challenge/run
/challenge/run
I'm back! Here's your flag:
pwn.college{E8SOQCUl3k0pPqgJ6yO9OWpx9Kf.QX2QDO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use fg command to resume suspended processes

## References 
None
