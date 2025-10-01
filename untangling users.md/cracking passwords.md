# Challenge Name
cracking passwords

## My solve
**Flag:** `pwn.college{cCYbxqGhOYxWP1RwXXORK7ISPau.QX3UDN1wyN0gjNzEzW}`

```bash
Connected!
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:21 100% 2/3 0.04642g/s 270.3p/s 270.3c/s 270.3C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{cCYbxqGhOYxWP1RwXXORK7ISPau.QX3UDN1wyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned to crack passwords using the john the ripper and using su to get the required flag

## References 
None
