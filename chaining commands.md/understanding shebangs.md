# Challenge Name
understanding shebangs
## My solve
**Flag:** `pwn.college{kDefh-noW5IIjs9jnB42jgXT2Nz.0VOzMDOxwyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~understanding-shebangs:~$ cat > /home/hacker/solve.sh <<'EOF'
#!/bin/bash
echo "hack the planet"
EOF
hacker@chaining~understanding-shebangs:~$ chmod +x /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ cat /home/hacker/solve.sh
#!/bin/bash
echo "hack the planet"
hacker@chaining~understanding-shebangs:~$ /challenge/run
Testing your script...
Perfect! Your flag:
Flag: pwn.college{kDefh-noW5IIjs9jnB42jgXT2Nz.0VOzMDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to use #! as a shebang which makes the script be treated as a program so we need not use bash to run the script

## References 
None
