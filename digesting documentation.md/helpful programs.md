# Challenge Name
helpful programs

## My solve
**Flag:** 'pwn.college{oVKfg7xIhxX2EsHPRjsQPqUbVEw.QX3IDO0wyN0gjNzEzW}'

```bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 723
hacker@man~helpful-programs:~$ /challenge/challenge -g 723
Correct usage! Your flag: pwn.college{oVKfg7xIhxX2EsHPRjsQPqUbVEw.QX3IDO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned about the --help argument to read certain directories not readable with man command

## References 
None
