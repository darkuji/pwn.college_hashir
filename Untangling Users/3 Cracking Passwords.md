# Cracking Passwords
### The challenge asks us to crack passwords


## My Solve
**Flag:** pwn.college{0HtWKxqPwmk1iQFcnBM0eL1K7lW.QX3UDN1wSO1EzNzEzW}
ran john /challenge/shadow-leak as per the instructions to get the
actual password of zardus. Obtained the password then used su zardus
to get access to his files and ran /challenge/run 



```
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
0g 0:00:00:17 0% 2/3 0g/s 264.7p/s 264.7c/s 264.7C/s national..rocket1
aardvark         (zardus)
1g 0:00:00:22 100% 2/3 0.04482g/s 261.0p/s 261.0c/s 261.0C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ --show
bash: --show: command not found
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{0HtWKxqPwmk1iQFcnBM0eL1K7lW.QX3UDN1wSO1EzNzEzW}
```

## What I Learned
Learned how to crack passwords


## References
Samar Nanda Boy