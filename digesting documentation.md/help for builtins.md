# Challenge Name
help for builtins

## My solve
**Flag:** `pwn.college{kuMyAfUwl3vsfX2LbnEdDfUjfMs.QX0ETO0wyN0gjNzEzW}`

```bash
hacker@man~help-for-builtins:~$ /challenge --help
bash: /challenge: Is a directory
hacker@man~help-for-builtins:~$ /challenge/challenge --help
bash: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "kuMyAfUw".
hacker@man~help-for-builtins:~$ /challenge --secret VALUE "kuMyAfUw"
bash: /challenge: Is a directory
hacker@man~help-for-builtins:~$  /challenge/challenge --secret VALUE "kuMyAfUw"
bash: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ challenge --secret kuMyAfUw
Correct! Here is your flag!
pwn.college{kuMyAfUwl3vsfX2LbnEdDfUjfMs.QX0ETO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
I didnt use the help command properly and instead used the argumement and kept calling the wrong path for challenge leading to multiple errors

## What I learned
I learned about builtins and the use of help

## References 
None
