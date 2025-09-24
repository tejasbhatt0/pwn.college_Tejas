# Implicit relative paths, from /
What the challenge is about / expects from you.

## My solve
**Flag:** `pwn.college{wbwQvyp42b68Q8kpCNbzWZMuAzl.QX5QTN0wiN2gjNzEzW}`

I went into the root directory using the cd command. Then I invoked the required command using it's path relative to the root directory, which is: "challenge/run". This gave me the flag.
```bash
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wbwQvyp42b68Q8kpCNbzWZMuAzl.QX5QTN0wiN2gjNzEzW}
```

## What I learned
I learned how to change directories and invoke commands using relative paths instead of using their absolute path everytime.

## Incorrect tangents
N.A.

## References
N.A.
