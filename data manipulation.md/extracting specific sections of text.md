# Challenge Name
extracting specific sections of text

## My solve
**Flag:** `pwn.college{QdMKVBYsyWIl80WgxK6I0SPwteD.01NxEzNxwyN0gjNzEzW}`

```bash
Connected!
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run
23672 p
24440 w
19515 n
20049 .
12220 c
29098 o
78 l
6345 l
13413 e
2419 g
26401 e
21385 {
22496 Q
17369 d
26304 M
26672 K
12960 V
11380 B
1333 Y
4493 s
28892 y
6826 W
10895 I
13599 l
10766 8
15999 0
17703 W
11779 g
21041 x
16301 K
30539 6
7282 I
8563 0
4803 S
22586 P
19169 w
3204 t
18313 e
2689 D
14452 .
32249 0
5899 1
381 N
21255 x
4180 E
32364 z
3945 N
22922 x
2074 w
29331 y
14887 N
3138 0
18452 g
6862 j
2935 N
27839 z
2976 E
23032 z
24186 W
18031 }
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d "\n"
pwn.college{QdMKVBYsyWIl80WgxK6I0SPwteD.01NxEzNxwyN0gjNzEzW}
```
## Incorrect tangents I went on
None

## What I learned
I learned  to extract specific columns using cut -d -f command

## References 
None
