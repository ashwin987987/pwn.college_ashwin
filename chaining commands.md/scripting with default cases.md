# Challenge Name
scripting with default cases

## My solve
**Flag:** `pwn.college{4RCZOa2X8q044gWnmeimYq5xH7N.01NzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~scripting-with-default-cases:~$ cat > /home/hacker/solve.sh <<'EOF'
#!/bin/bash
# Print "college" if first arg is "pwn", otherwise print "nope"
if [ "$1" = "pwn" ]; then
  printf '%s\n' "college"
else
  printf '%s\n' "nope"
fi
EOF
hacker@chaining~scripting-with-default-cases:~$ chmod +x /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{4RCZOa2X8q044gWnmeimYq5xH7N.01NzMDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use else in scripts

## References 
None
