# Challenge Name
symbolic links

## My solve
**Flag:** pwn.college{8ZnGbf-deFkG0F3m9EFPo6xteTl.QX5ETN1wyN0gjNzEzW}

```bash
hacker@commands~linking-files:~$ rm /home/hacker/not-the-flag
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ cat /challenge/catflag
#!/opt/pwn.college/bash

fold -s <<< "About to read out the /home/hacker/not-the-flag file!"
cat /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{8ZnGbf-deFkG0F3m9EFPo6xteTl.QX5ETN1wyN0gjNzEzW}
```
## Incorrect tangents I went on
I tried symbolic linking without removing the fake file. I also catted the file when i just needed to specify the name resulting in errors

## What I learned
I learned about symbolic links are the way they are used to soft link files
## References 
None
