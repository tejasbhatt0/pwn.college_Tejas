# Listing files
The challenge teaches us about how to list files in the directory you are currently in using "ls".

## My solve
**Flag:** `pwn.college{U048654QgOen_u51t0aoW5xIx64.QX4IDO0wiN2gjNzEzW}`
First, I went to the "/challenge" directory using cd. Then I listed it's contents using "ls". Then I invoked "/challenge/633-renamed-run-29581" to get the flag.

```bash
hacker@commands~listing-files:~$ cd /challenge
hacker@commands~listing-files:/challenge$ ls
633-renamed-run-29581  DESCRIPTION.md
hacker@commands~listing-files:/challenge$ /challenge/633-renamed-run-29581
Yahaha, you found me! Here is your flag:
pwn.college{U048654QgOen_u51t0aoW5xIx64.QX4IDO0wiN2gjNzEzW}
```

## What I learned
I learned how to list the files in a directory using "ls".

## Incorrect tangents
N.A.

## References
N.A.
