# Challenge Name
scripting with arguments
## My solve
**Flag:** `pwn.college{cORyAA1XGCxohCiYvK5S6XkWqb_.0VNzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~scripting-with-arguments:~$ cat > /home/hacker/solve.sh <<'EOF'
#!/bin/bash
printf '%s %s\n' "$2" "$1"
EOF
hacker@chaining~scripting-with-arguments:~$ chmod +x /home/hacker/solve.sh
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{cORyAA1XGCxohCiYvK5S6XkWqb_.0VNzMDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned that arguments can be added to scripts using $1,$2 etc

## References 
None
