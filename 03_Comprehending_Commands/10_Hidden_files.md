# Hidden Files
The challenge teaches us about hidden files, how they don't show up when we invoke "ls" because they start with a "." and how we can list them the using "ls -a".

## My solve
**Flag:** `pwn.college{oR7CxibnaKfkTqRj0zStViv7T9O.QXwUDO0wiN2gjNzEzW}`
I used "ls -a" to show all files in the root directory (even hidden files). This showed me the ".flag-24502148869902" file. Then I used "cat" to read that file, upon which it gave me the flag.

```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-24502148869902  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-24502148869902
pwn.college{oR7CxibnaKfkTqRj0zStViv7T9O.QXwUDO0wiN2gjNzEzW}
```

## What I learned
I learned how to list hidden files using the "ls -a" command.

## Incorrect tangents
N.A.

## References
N.A.
