# Comparing Files
The challenge teaches us how the diff command can be used to tell the differences between two files.

## My solve
**Flag:** `pwn.college{coTtkHNWqV4rzs6qpRqj7bd1BSe.01MwMDOxwiN2gjNzEzW}`
I used "diff" with "/challenge/decoys_only.txt" and "/challenge/decoys_and_real.txt" as it's two arguments. This gave me the real flag that was in the "decoys_and_real.txt" file.


```bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
98a99
> pwn.college{coTtkHNWqV4rzs6qpRqj7bd1BSe.01MwMDOxwiN2gjNzEzW}
```

## What I learned
I learned how to use the "diff" command to compare two files.

## Incorrect tangents
N.A.

## References
N.A.
