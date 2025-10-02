# Challenge Name
detaching and attaching tmux

## My solve
**Flag:** `pwn.college{wuHdSNg2wh_LjvXvl9Iid62Ti9j.0VO4IDOxwyN0gjNzEzW}`

```bash
Connected!
Connected!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux a
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{wuHdSNg2wh_LjvXvl9Iid62Ti9j.0VO4IDOxwyN0gjNzEzW}
Congratulations, here is your flag: pwn.college{wuHdSNg2wh_LjvXvl9Iid62Ti9j.0VO4IDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to detach and attach in tmux using ctrl B + d and tmux a

## References 
None
