# Home Sweet Home
It teaches us about how every linux system has a home directory, and how /home/hacker path (in our case) is abbreviated as "~".

## My solve
**Flag:** `pwn.college{k0txYWRMkQqm2N30pJSTTQrFA3F.QXzMDO0wiN2gjNzEzW}`

I invoked "/challenge/run" with the argument "~/~" which, when expanded, means "/home/hacker/~". Then it gave me the flag.

```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/~
Writing the file to /home/hacker/~!
... and reading it back to you:
pwn.college{k0txYWRMkQqm2N30pJSTTQrFA3F.QXzMDO0wiN2gjNzEzW}
```

## What I learned
I learned how every linux system has a home directory and its abbreviation (in our case "/home/hacker" is abbreviated as "~")

## Incorrect tangents
N.A.

## References
N.A.
