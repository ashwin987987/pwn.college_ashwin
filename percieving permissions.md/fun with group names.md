# Challenge Name
fun with group names

## My solve
**Flag:** `pwn.college{wsWnNPuZ76RjjSWG7diCNN2ivbH.QXycjM1wyN0gjNzEzW}`

```bash
Connected!
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp9551) groups=1000(grp9551)
hacker@permissions~fun-with-groups-names:~$ chgrp grp9551 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{wsWnNPuZ76RjjSWG7diCNN2ivbH.QXycjM1wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use id command to get access to every group a user is part of and that group name can be different from user name

## References 
None
