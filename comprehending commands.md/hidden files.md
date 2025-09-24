# Challenge Name
hidden files

## My solve
**Flag:**pwn.college{ISP1fwuMMnSO7L1BJ4ZRu7Obldv.QXwUDO0wyN0gjNzEzW}

```bash
Connected!
hacker@commands~hidden-files:~$ ls -a /
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-214853047629699  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-214853047629699
pwn.college{ISP1fwuMMnSO7L1BJ4ZRu7Obldv.QXwUDO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about hidden files starting with . which are not displayed by ls. we need to use ls -a to display them

## References 
None
