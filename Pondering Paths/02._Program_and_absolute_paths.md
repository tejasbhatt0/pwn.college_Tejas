# Program and absolute paths
What the challenge is about / expects from you.

## My solve
**Flag:** `pwn.college{sh9pHljareBCxSc2TdfV7VoqSQA.QX1QTN0wiN2gjNzEzW}`

It explores a slightly more complicated absolute path than the previous challenge. This time the "run" program is in the "challenge" directory, which in turn is in the "root" directory. Thus we can invoke it by running the command "/challenge/run".
```bash
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{sh9pHljareBCxSc2TdfV7VoqSQA.QX1QTN0wiN2gjNzEzW}
```

## What I learned
I learned to traverse directories using absolute paths.

## Incorrect tangents
N.A.

## References
N.A.
