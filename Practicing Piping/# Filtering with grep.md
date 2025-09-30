# Filtering with grep
### The challenge asks us to use grep -v to filter search output


## My Solve
**Flag:** pwn.college{wy1lpd4rmuxIJ_dmvv8NijTaYdm.0FOxEzNxwSO1EzNzEzW}
Used the /challenge/run | grep -v DECOY command to directly search the 
/challenge/run file and filter out any words with decoy


```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{wy1lpd4rmuxIJ_dmvv8NijTaYdm.0FOxEzNxwSO1EzNzEzW}
```

## What I Learned
I learned how we can filter out searches with a keyword using grep -v

## References
None