# Redirecting More Output
### The challenge asks us to use > to redirect output of a program to another file


## My Solve
**Flag:** pwn.college{UpL4xNlwcyQwNVbdMSE8R5KUW9X.QX1YTN0wSO1EzNzEzW}
I first redirected the output of /challenge/run to myflag file using >
after which i opened the myflag file



```
hacker@piping~redirecting-more-output:/tmp$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:/tmp$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{UpL4xNlwcyQwNVbdMSE8R5KUW9X.QX1YTN0wSO1EzNzEzW}
```

## What I Learned
I learned how we can use > to redirect output of many commands
and not only echo

## References
None