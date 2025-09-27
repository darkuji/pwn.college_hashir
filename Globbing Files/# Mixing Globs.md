# Mixing Globs
### The challenge asks us to use the different globs we have learnt so far


## My Solve
**Flag:** pwn.college{EA5Vugz1UGLIGf1vkDGYtdxFbuA.QX1IDO0wSO1EzNzEzW}
I noticed that unlike the rest of the files, the files to be searched were
the only ones that started with c e and p so i used the [] argument with cep
indicating i needed files c e p and used * after it coz the further part of it 
could be anything


```
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ pwn.college{kdxEhacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{EA5Vugz1UGLIGf1vkDGYtdxFbuA.QX1IDO0wSO1EzNzEzW}
```

## What I Learned
I learned how we can use different types of file globbing together according
to our convenience in a Linux environment 

## References
None