# Challenge Name
scripting with multiple conditions
## My solve
**Flag:** `pwn.college{M0iG1Kg0wgqx16azvlduI_CUXJq.0FOzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~scripting-with-multiple-conditions:~$ cat > /home/hacker/solve.sh <<'EOF'
#!/bin/bash
if [ "$1" = "hack" ]; then
  printf '%s\n' "the planet"
elif [ "$1" = "pwn" ]; then
  printf '%s\n' "college"
elif [ "$1" = "learn" ]; then
  printf '%s\n' "linux"
else
  printf '%s\n' "unknown"
fi
EOF
hacker@chaining~scripting-with-multiple-conditions:~$  chmod +x /home/hacker/solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$  /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{M0iG1Kg0wgqx16azvlduI_CUXJq.0FOzMDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use if elif else ladder in scripts

## References 
None
