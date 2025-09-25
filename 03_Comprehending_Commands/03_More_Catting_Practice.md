# More Catting Practice
This challenge expects us to learn that cat can also be invoked using the abolute path to a file to read it.

## My solve
**Flag:** `pwn.college{I9bdl7HC1kpQV9nNIQPnhrQB3yO.QXwITO0wiN2gjNzEzW}`

I tried to change my directory but it told me that it was not allowed for this challenge. Then it also told me where the absolute path of the flag was. Then I read the flag using it's absolute path.
```bash
hacker@commands~more-catting-practice:~$ cd /
You used 'cd'! In this level, I don't allow you to change the working directory
--- you MUST chase pass 'cat' the absolute path of where I put it on the
filesystem (which is /usr/lib/clang/flag).
hacker@commands~more-catting-practice:~$ cat /usr/lib/clang/flag
pwn.college{I9bdl7HC1kpQV9nNIQPnhrQB3yO.QXwITO0wiN2gjNzEzW}
```

## What I learned
I learned that the "cat" command can also be invoked by passing the absolute path to a file as it's argument, to read it.

## Incorrect tangents
N.A.

## References
N.A.
