# Grepping Errors
### The challenge asks us to use >& to convert data streams


## My Solve
**Flag:** pwn.college{o4EM0dxoQx4pQ9VqVm8rITysmA8.QX1ATO0wSO1EzNzEzW}
I ran the /challenge/run 2>& 1 command to redirect output and grep
pwn to search for the flag


```
hacker@piping~grepping-errors:~$ /challenge/run 2>& 1 | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{o4EM0dxoQx4pQ9VqVm8rITysmA8.QX1ATO0wSO1EzNzEzW}
pwned
pwning
pwns
pwn
```

## What I Learned
Learned how to grep error files directly using >&

## References
None