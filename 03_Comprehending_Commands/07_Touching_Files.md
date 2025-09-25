# Touching Files
The challenge teaches us to create files using the "touch" command.

## My solve
**Flag:** `pwn.college{EneR8Hip9MJMU42JcOOXx1zPh1W.QXwMDO0wiN2gjNzEzW}`
I created two files using "touch /tmp/pwn" and "touch /tmp/college" separately and then invoked "/challenge/run" to get the flag.

```bash
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.TpSOPGOVKK
hacker@commands~touching-files:/tmp$ touch /tmp/pwn
hacker@commands~touching-files:/tmp$ touch /tmp/college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.TpSOPGOVKK
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{EneR8Hip9MJMU42JcOOXx1zPh1W.QXwMDO0wiN2gjNzEzW}
```

## What I learned
I learned how to create files using the "touch" command.

## Incorrect tangents
N.A.

## References
N.A.
