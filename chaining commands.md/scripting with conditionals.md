# Challenge Name
scripting with conditionals

## My solve
**Flag:** `pwn.college{QNTf5VrSnL2YxxhaXx7uZYD8vGo.0lNzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~scripting-with-conditionals:~$ cat > /home/hacker/solve.sh <<'EOF'
#!/bin/bash
if [ "$1" = "pwn" ]; then
  printf '%s\n' "college"
fi
EOF
hacker@chaining~scripting-with-conditionals:~$  chmod +x /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{QNTf5VrSnL2YxxhaXx7uZYD8vGo.0lNzMDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use conditions using if and closing it with fi

## References 
None
