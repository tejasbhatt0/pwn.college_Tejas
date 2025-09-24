# Position yet elsewhere
The challenge is about changing directories using the cd command with an absolute path argument, and also to invoke certain commands from specific directories.

## My solve
**Flag:** `pwn.college{oxdNfbt4stKBQ40hX9mq35CcJv5.QX4QTN0wiN2gjNzEzW}`

I invoked the /challenge/run command but it told me that I was running it from the incorrect directory. It told me to go to /etc/apt/sources.list.d and then run the command. I did that and got the flag.
```bash
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /etc/apt/sources.list.d directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /etc/apt/sources.list.d
hacker@paths~position-yet-elsewhere:/etc/apt/sources.list.d$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{oxdNfbt4stKBQ40hX9mq35CcJv5.QX4QTN0wiN2gjNzEzW}
```

## What I learned
I learned how to traverse directories using the cd command with the agrument of an absolute path.

## Incorrect tangents
N.A.

## References
N.A.
