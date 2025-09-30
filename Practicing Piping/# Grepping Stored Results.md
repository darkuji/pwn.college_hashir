# Grepping Stored Results
### The challenge asks us to redirect output and search for the flag


## My Solve
**Flag:** pwn.college{YyTLDUYX-9ZSp6My1cE1i_0xPhO.QX4EDO0wSO1EzNzEzW}
I first redirected the ouput of /challenge/run to /tmp/data.txt using 
the > command after which i grepped with the keyword pwn since the
flag starts with pwn.college


```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn /tmp/data.txt
pwns
pwning
pwned
pwn.college{YyTLDUYX-9ZSp6My1cE1i_0xPhO.QX4EDO0wSO1EzNzEzW}
pwn
```

## What I Learned
I learned nothing new

## References
None