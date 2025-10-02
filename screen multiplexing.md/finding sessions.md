# Challenge Name
finding sessions

## My solve
**Flag:** `pwn.college{A5HHe9g35ACxM0I1Z8B3xbrv1f4.01N4IDOxwyN0gjNzEzW}`

```bash
connected!
hacker@terminal-multiplexing~finding-sessions:~$ screen -r
There are several suitable screens on:
        150.pts-0.terminal-multiplexing~launching-screen        (Remote or dead)
        139.pts-0.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        176.pts-2.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        144.session_5caf995c2e529e71    (Detached)
        147.session_3fef0ca09545dc0d    (Detached)
        150.session_b8ffae2d538433a8    (Detached)
        191.pts-3.terminal-multiplexing~finding-sessions        (Detached)
        216.pts-5.terminal-multiplexing~finding-sessions        (Detached)
Type "screen [-d] -r [pid.]tty.host" to resume one of them.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 144
[detached from 144.session_5caf995c2e529e71]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 147
[detached from 147.session_3fef0ca09545dc0d]
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{A5HHe9g35ACxM0I1Z8B3xbrv1f4.01N4IDOxwyN0gjNzEzW}
pwn.college{A5HHe9g35ACxM0I1Z8B3xbrv1f4.01N4IDOxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to search for screens with their respective PID

## References 
None
```


None
