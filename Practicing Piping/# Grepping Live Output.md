# Grepping Live Output
### The challenge asks us to search for the flag directly from the file 


## My Solve
**Flag:** pwn.college{QhAzRSDIh5s7pNW0ZvQNuvXRZsx.QX5EDO0wSO1EzNzEzW}
I used the | operator to search directly from the /challenge/run 
program with the grep command with argument as pwn since the flag
starts with pwn.college

```
hacker@piping~grepping-live-output:~$ /challenge/run | grep pwn
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stdout : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stdout!
[PASS] Success! You have satisfied all execution requirements.
pwns
pwning
pwn
pwned
pwn.college{QhAzRSDIh5s7pNW0ZvQNuvXRZsx.QX5EDO0wSO1EzNzEzW}
```

## What I Learned
I learned how we can use the grep command to search from a file 
directly from the main file using | without having to involve another
file in which the output is stored first

## References
None