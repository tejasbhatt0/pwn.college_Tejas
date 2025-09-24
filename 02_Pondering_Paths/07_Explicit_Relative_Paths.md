# Explicit Relative Paths, from /
The challenge teaches us to use explicit relative paths by using ".".

## My solve
**Flag:** `pwn.college{kqSQYKeXyOEgGYsMbMOBVM6cPBm.QXwUTN0wiN2gjNzEzW}`

First I entered the root directory. Then I invoked the command using it's explicit relative path - "./challenge/run".
```bash
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kqSQYKeXyOEgGYsMbMOBVM6cPBm.QXwUTN0wiN2gjNzEzW}
```

## What I learned
I learned how to use explicit relative paths.

## Incorrect tangents
N.A.

## References
N.A.
