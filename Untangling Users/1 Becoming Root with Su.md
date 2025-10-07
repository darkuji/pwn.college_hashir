# Becoming Root with Su
### The challenge asks us to use su command to become root


## My Solve
**Flag:** pwn.college{sV1Nh3m8M0ZaD6mTQPT_i3B4iAx.QX1UDN1wSO1EzNzEzW}
Used su then entered the password to access the files. Ran 
cat /flag to obtain the flag

```
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{sV1Nh3m8M0ZaD6mTQPT_i3B4iAx.QX1UDN1wSO1EzNzEzW}
root@users~becoming-root-with-su:/home/hacker#
```

## What I Learned

Learned how we can become root using the su command

## References
None