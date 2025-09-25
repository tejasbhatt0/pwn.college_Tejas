# Moving Files
The challenge teaches us how to move files between directories using the "mv" command.

## My solve
**Flag:** `pwn.college{cQehPV9XKk9nwElqLMjQI4zyDS-.0VOxEzNxwiN2gjNzEzW}`
I used the "mv" command to move the flag file from "/flag" to "/tmp/hack-the-planet" by passing these in as the first and second arguments respectively, to the "mv" command.

```bash
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{cQehPV9XKk9nwElqLMjQI4zyDS-.0VOxEzNxwiN2gjNzEzW}
```

## What I learned
I learned how to move files between directories using the "mv" command. It takes the first argument as the current file path, and the second argument as the file path you want it to have (i.e. moved to).

## Incorrect tangents
N.A.

## References
N.A.
