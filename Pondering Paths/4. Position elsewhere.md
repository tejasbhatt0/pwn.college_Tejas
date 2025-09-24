# Position elsewhere
The challenge is about changing directories using the cd command with an absolute path argument, and also to invoke certain commands from specific directories.

## My solve
**Flag:** `pwn.college{wV4Za4MbietNvzwMvQwTjFEVh3S.QX3QTN0wiN2gjNzEzW}`

I invoked the /challenge/run command but it told me that I was running it from the incorrect directory. It told me to venture to /usr/include and then run the command. I did that and got the flag.

```bash
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/include directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/include
hacker@paths~position-elsewhere:/usr/include$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wV4Za4MbietNvzwMvQwTjFEVh3S.QX3QTN0wiN2gjNzEzW}
```

## What I learned
I learned how to traverse directories using the cd command with the agrument of an absolute path.

## Incorrect tangents
N.A.

## References
N.A.
