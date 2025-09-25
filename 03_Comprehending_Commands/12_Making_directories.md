# Making Directories
The challenge expects us to understand how to make directories using the "mkdir" command.

## My solve
**Flag:** `pwn.college{U3bLLTZIm1eH5mJWOtdMHs5neKU.QXxMDO0wiN2gjNzEzW}`
I used "mkdir" command with the argument of the path I wanted to create the directory at i.e. "/tmp/pwn". Then I created the file "college" using "touch /tmp/pwn/college". After this I ran "/challenge/run" which gave me the flag.

```bash
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:~$ touch /tmp/pwn/college
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{U3bLLTZIm1eH5mJWOtdMHs5neKU.QXxMDO0wiN2gjNzEzW}
```

## What I learned
I learned how to make directories using the command "mkdir"

## Incorrect tangents
N.A.

## References
N.A.
