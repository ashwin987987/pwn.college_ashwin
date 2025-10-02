# Challenge Name
reading shell scripts

## My solve
**Flag:** `pwn.college{ANcNM8sjdl2nz3G41j_Yl94y4UE.0lMwgDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~reading-shell-scripts:~$ /challenge/run

Connected!
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ printf '%s\n' 'hack the PLANET' | /challenge/run
CORRECT! Your flag:
pwn.college{ANcNM8sjdl2nz3G41j_Yl94y4UE.0lMwgDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to read shell scripts using cat and then how to give the value of the argument to get the desired output

## References 
None
