# Challenge Name
redirecting script output

## My solve
**Flag:** `pwn.college{s_5YLMs9dxiLybFpXdMFy077-oV.QX4ETO0wyN0gjNzEzW}`

```bash
Connected!
hacker@chaining~redirecting-script-output:~$ cat > x.sh <<'EOF'
/challenge/pwn
/challenge/college
EOF
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{s_5YLMs9dxiLybFpXdMFy077-oV.QX4ETO0wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned that piping output of scripts to a file can be done using | 

## References 
None
