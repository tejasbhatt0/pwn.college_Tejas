# Implicit Relative Paths
This challenge teaches us how to invoke a program by using it's relative path and not it's name directly.

## My solve
**Flag:** `pwn.college{helloworld}`

I first went to root by using "cd /" and then inside the challenge directory using "cd ./challenge". Then I invoked the command using "./run".
```bash
hacker@paths~implicit-relative-path:/challenge$ cd /
hacker@paths~implicit-relative-path:/$ cd ./challenge
hacker@paths~implicit-relative-path:/challenge$ run
bash: run: command not found
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{0K1Oh0QbVlJitxRL-IKnDT4Mot1.QXxUTN0wiN2gjNzEzW}
```

## What I learned
I learned to invoke the command (while being present in it's directory) by using it's explicit relative path using "./" and not just it's name.

## Incorrect tangents
N.A.

## References
N.A.
