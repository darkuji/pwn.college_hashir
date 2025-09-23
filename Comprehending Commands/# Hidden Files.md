# Hidden Files
### This challenge asks us to reveal the hidden files using the -a command


## My Solve
**Flag:** pwn.college{ItClNxCZBlSA3P6vgJLZ8Cua668.QXwUDO0wSO1EzNzEzW}
First i used ls -a to reveal the names of files that started with a '.'
then i used the cat command along with the name of the flag file to read
it and obtain the flag


```
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-70891047725372  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-70891047725372
pwn.college{ItClNxCZBlSA3P6vgJLZ8Cua668.QXwUDO0wSO1EzNzEzW}
```

## What I Learned
I learned how in a Linux environment the terminal by default ignores
the file whose names start with a '.' and in order to access them we 
need to pass the argument '-a' along with the ls command

## References
None