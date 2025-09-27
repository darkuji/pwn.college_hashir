# Searching for manuals
### The challenge asks us to find the argument with which we need to run the man command


## My Solve
**Flag:** pwn.college{4PhcjT9IXFytnA4mXccKz2u5tv-.QX2EDO0wSO1EzNzEzW}
I first used the man man command and figured that i need to use the -k 
command to search for a keyword then used it with flag to find out the files
where i found the hcjytnmccz file of which i read the manual and found out
that i need to use the --hcjytn 494 argument along with /challenge/challenge
for the system to print the flag


```
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k flag
dpkg-buildflags (1)  - returns build flags to use during package build
Dpkg::BuildFlags (3perl) - query build flags
fegetexceptflag (3)  - floating-point rounding and exception handling
fesetexceptflag (3)  - floating-point rounding and exception handling
hcjytnmccz (1)       - print the flag!
i386 (8)             - change reported architecture in new program environment and/or set personality flags
ioctl_iflags (2)     - ioctl() operations for inode flags
linux32 (1)          - change reported architecture in new program environment and/or set personality flags
linux64 (1)          - change reported architecture in new program environment and/or set personality flags
pcap-config (1)      - write libpcap compiler and linker flags to standard output
security_compute_av_flags (3) - query the SELinux policy database in the kernel
security_compute_av_flags_raw (3) - query the SELinux policy database in the kernel
set_matchpathcon_flags (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure the behaviour...
set_matchpathcon_invalidcon (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure the beha...
set_matchpathcon_printf (3) - set flags controlling the operation of matchpathcon or matchpathcon_index and configure the behaviou...
setarch (1)          - change reported architecture in new program environment and/or set personality flags
setarch (8)          - change reported architecture in new program environment and/or set personality flags
x86_64 (8)           - change reported architecture in new program environment and/or set personality flags
hacker@man~searching-for-manuals:~$ man hcjytnmccz
hacker@man~searching-for-manuals:~$ /challenge/challenge --hcjytn 494
Correct usage! Your flag: pwn.college{4PhcjT9IXFytnA4mXccKz2u5tv-.QX2EDO0wSO1EzNzEzW}
```

## What I Learned
I learned how the man man command gives us the manual of the man command itself
where we can find different arguments we can give with man to perform a particular task


## References
None