# Challenge Name
adding commands

## My solve
**Flag:** `pwn.college{8jlBE5GRW2FEWCkK62c6D4jqi53.QX2cjM1wyN0gjNzEzW}`

```bash
Connected!
hacker@path~adding-commands:~$ mkdir -p /home/hacker/bin
hacker@path~adding-commands:~$ cat > /home/hacker/bin/win <<'EOF'
#!/bin/bash
read -r FLAG < /flag
printf '%s\n' "$FLAG"
EOF
hacker@path~adding-commands:~$ chmod +x /home/hacker/bin/win
hacker@path~adding-commands:~$ PATH=/home/hacker/bin /challenge/run
Invoking 'win'....
pwn.college{8jlBE5GRW2FEWCkK62c6D4jqi53.QX2cjM1wyN0gjNzEzW
```
## Incorrect tangents I went on
None

## What I learned
I learned to add commands in specific paths

## References 
None
