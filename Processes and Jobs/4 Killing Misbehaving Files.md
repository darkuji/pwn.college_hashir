# Killing Misbehaving Files
### The challenge asks us to kill files interfering with our work


## My Solve
**Flag:** pwn.college{AvtnOOFIB8pwdtLOXsX95_qfoL8.0FNzMDOxwSO1EzNzEzW}
Used ps -ef to list out all the processes that were running. Accidentally 
killed the wrong process then used 142 to kill the right one then ran 
/challenge/run which sent the flag along with a few decoys to the temp
file for which i opened a new window and catted the temp file and ran
/challenge/run again which this time gave only the original flag


```
hacker@processes~killing-misbehaving-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 16:37 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 16:37 ?        00:00:00 /run/dojo/bin/sleep 6h
root         137       1  0 16:37 ?        00:00:00 /bin/bash /challenge/.init
root         138       1  0 16:37 ?        00:00:00 /bin/bash /challenge/.init
root         139       1  0 16:37 ?        00:00:00 su -c exec /challenge/decoy > /tmp/flag_fifo hacker
root         140     137  0 16:37 ?        00:00:00 sleep 6h
root         141     138  0 16:37 ?        00:00:00 sleep 6h
hacker       142     139  0 16:37 ?        00:00:00 /usr/bin/python /challenge/decoy
hacker       144       0  1 16:37 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       150     144  0 16:37 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       159     150  0 16:37 pts/0    00:00:00 ps -ef
hacker@processes~killing-misbehaving-processes:~$ kill 139
bash: kill: (139) - Operation not permitted
hacker@processes~killing-misbehaving-processes:~$ kill 142
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!
hacker@processes~killing-misbehaving-processes:~$ /challenge/run
Sending the flag to /tmp/flag_fifo!

hacker@processes~killing-misbehaving-processes:~$ cat /tmp/flag_fifo
pwn.college{MwXmGGzsdT3Ec3qh4-dWYseq6Wso8xnww.HR9W.l6Bym9fu}
pwn.college{0HsJW9ddsBA6gtun5c82Xs9CMNKX-scfm7Y9lgZrb40oYG1}
pwn.college{zix-wZmpSbxv6SP24.4laBs1-s6nvREvUbTD4NQlmV0gkPq}
pwn.college{2emSgmQ.LnlAucxnTIM2aTmaO9sSScQYAT-pnw1o0AX0.nz}
pwn.college{S.EAuIOmdWlW4b6a9aXwqPQrd.Ou5uaUW2D4VLHw0mkHupw}
pwn.college{MUM6Zb8uekbqktr.aD1nMygJzNrU-LZPHDjrH4DlFspe3f9}
pwn.college{ONnw-xwNHKYy4taeSb4Lv3Xqng1km6ApGop5UgPUIGFl5Q5}
pwn.college{tByiTEwzaxgGmYZ5iktbNvetwvVcpUSYVtoTpwN7Dvvj8xT}
pwn.college{ItXDAFIQ3z.a1i1V6iD.O8oIUyelx9kfv0yN00c9Oi9KGYx}
pwn.college{xPadIk5xX1jqSsrdW4Ki2S5FcjM.GQ0zaZ-Xx-iA2cYo9V2}
pwn.college{928fblaspsPzWJPofLr3S9TWlge28fBEk59ymt5oWEcK16P}
pwn.college{F.W5aoWEPozanmfXQUX8F7nrymGRGQCIviwLHxElYJ9DIZA}
pwn.college{4qu5NvVyolJgWmHgVin3v4wyF.eDTq.BQnSh4r6QVxNwdNI}
pwn.college{ag7n-qdU61Bc98tIDi9Fl2t9Yl-LFws3PzKWu5.IrrLIKYi}
pwn.college{yKaALhMRP.krSYREbeUxgrRyta46B5l-mya5a3XiJa7NY.-}
pwn.college{o-B8lYRDK2eZxlfBn-bk.Nv8LCyZ57jSeuyltWBjwWt.Md7}
pwn.college{HAIhzAPuTIJjNoUyTSPECrLKvQcVLDuN1GbJ5EPshSXalKi}
pwn.college{83jJDiMy.e19kqE4iuxsx6P5QtAd1YbLLBXZiviXumuwQuJ}
pwn.college{HvxNdB8rP2m5xlMxLvXSUq0L5INnX9H7Jq7JQPAL66QnQFV}
pwn.college{LfEX6pgzyioMzpk53pemF4r5-ZTmxPaIhtnHkXT2XsVSRbC}
pwn.college{LLX.onBgHWZ.Nwo5PxYK-4TzTVbFZrd-1kUA2JWc-PIZel2}
pwn.college{4iaZqi1CAMS7OqFwqYRR78pvPYNoYePORmw5NAKT6EBKLpU}
pwn.college{C4qYDSPn.96HO8KCyYEWvw4gmm2-.XmE2pu4SKhFMtVEjcB}
pwn.college{8.NTDLWS8l-VKfexHuZ-5yISO5VdXIkr0lWLS5s2-ESU3bi}
pwn.college{u.HGCLvUtu1q1tVQNy8MkCvFYlFmhrK9jgTCdYjC--v-j0n}
pwn.college{5eRZhh5AAFTc7TJCYXBTmDWdeAFpX7XZnBQRwNG9FfZXpo0}
pwn.college{sVIN8.tiIv4.iKT3Vsr44d.2xxuf6pD0cL9BYeHmDSIzVhj}
pwn.college{Jupn2CeKogaLla2.nQsN29eO2rOiusVP-MgylEhQjwRaG0o}
pwn.college{1YuQLg4g-jZZU0nDryF3bTJyaxtGRZ9R3oIneWa2..VxOqO}
pwn.college{q6c8PNhIl8XUyE.CnU8bDdhsYvGMKjpqwMSdq-CKDF.LhhT}
pwn.college{9AQixct.lkS4XbddeA3QP7cxA7W5Ggp1P9e5Ql1Pk4NaAiV}
pwn.college{13P2b.nwutTrRsEBwV8kvgkQhpRV493xTk84Uz9OqhsETVq}
pwn.college{JWGp5SN.6xnaG9hmUGjMBc3BPRdIY9YSSz9-yr9BtXQ4Wo4}
pwn.college{9fK1puqIPBuwxWFknS6XJkgb2farap2x2ICK7kBZhVjAz0-}
pwn.college{xylbr8OUdLTkFk97fpGPA-ekU1RwALzefv7a9KKl3X0dy5d}
pwn.college{KJy.UPosXXuoqAcI3bpMZRKvXZpUjXOspsFG-ZZovpn89FT}
pwn.college{IYt-53BsY1cZmxFJx.0D3i2kWv2AaDziuDg0h3XhDGRkl6o}
pwn.college{VFBKiXll5s2e7Tjtipx73425G9vVtImHE4-UfXbtNCZyAN8}
pwn.college{jA-7Ru6T-aobBK.LexBCvc4ywGDsBq8T7wX3H5KX.6THu6V}
pwn.college{YeUCOu8pa90Ki-.OY3vHGjm01TuAdgsiQXfseGGGq-nnOV2}
pwn.college{LVTCQtWm8ZTYH.LDWqXTdrfGAAqx191HxRTiAB0qX2ejEpw}
pwn.college{7.8cVbYIVQjmHPOojsjpvRvAI9Fp1a4lqLh.k6AWU7DlYA-}
pwn.college{WKkOL92uZA6CKrYX3u8K7Te4j-njmxLPPygOkqcwxaEO7Wa}
pwn.college{RmqgELpmXlCdcEJ6HIw2QT3FA6Tjllo7MQVtGQJ1DlvSmku}
pwn.college{p-xeI-P-tmYwC16ytDlBZDfOkk1HTNi3Q6HcP.Zl5NL2bWK}
pwn.college{3XKIQDXUoc911iCFr2b8Y-p3or3sE97G.Jg-gvRmzHvOIyf}
pwn.college{.inrIlroO99hfDrXajamgDjo85WdpFYz5C9uDpeT295unr3}
pwn.college{hW8ElNGZnPg.xEYiQD5moB9QovdSoIBJ9CaPzEZ-FlVdj9C}
pwn.college{S2IJfk13wEWimcRb0C77CcJdNE-sZrMvg8H2gOrWKL3NeR-}
pwn.college{cTwY.xzkNbWlcb1M9QnKE9n.rKmAvkDrcK5cgLlJJOzFBY3}
pwn.college{HllCA7-.H3NCI2RxPlmkvMM3qLChoVCU27FvrcbGtpZ7es9}
pwn.college{PVRoD7-Q7ONMhqlIxM8p6Tf7jMAv0xjBSTw-yc.QkjdzGcg}
pwn.college{OHuLF22zrwFxa5O6s3PTZS65Tql-gI3Y0AFZpIxGt4yRmX0}
pwn.college{IDKus0zl6eG4wZ7epmuDoZc6fGr6S.HjlO2ulOI2ePOlfbm}
pwn.college{gLy17ZmLenFBCR.8i.MouBk-44ovqOO9hdngBaSQhBaun69}
pwn.college{fMiSgS60nkn2HhTMFuPWyAlO76MRTl8av0oeYqLDJWT7hYQ}
pwn.college{ZEZLHZhkQ0ZXKiA1CynV6gi23v69OeEc20hGQxQRuovGNtT}
pwn.college{Z0MTNDJQvp0SrsL4L9iGMiFgaT8YThTIx.MPepAGj.vCDi6}
pwn.college{y6U1lAqr6Ajc3n736laxi0F8XWv-Bt2RlqEcISI2EreqN7n}
pwn.college{py9k.gnRIY-NhFTbrPp863Mf4pK6hYyO25jIGJ8R2fhV0.r}
pwn.college{n3c3LAta9kNSkXbx7mUld4eevmEcCIEUs1ZeRDyZeKoSCp2}
pwn.college{owclljkHM7dLtnbT3g6X1sD0ynEazVnu3kynFNCphvz.odL}
pwn.college{KBGNr0gXUL.G9nVFCkkY14piNNvMX8q9npuKB38Njpe-uuV}
pwn.college{A3tA9x1XXmfTk0nf75XDrDnT0Ouu2L0q.fxlJj1ZJPFcfUj}
pwn.college{GKQcLaCPTZsM9K.9OlPfzQ0KIIKmmSWyl8q.093rD5zShj8}
pwn.college{jQNTjD0yH57e30lIxLfcBeWpDyDxCc9hkb4tyR98tIMG2Gc}
pwn.college{BHr4Uqo3HahubbfGEZvBXbhjXPfVLUFnaveBfhFs03-DGFY}
pwn.college{C4zMAvjgFUfUqYaR8cNNHagvq-Fv5X3Fzyh8V19dTCMSkzm}
pwn.college{OF9tXjAaZd8MkMQkXp3.TVYpXj53PnFzVM5Dbpx0OCwQDVO}
pwn.college{WRVcdwE7kCTkeAzhQitmMmRL.qqZEKoavgxifSfZSNaQ5CC}
pwn.college{FtgkjPIzMkEvtonmmoqjNQTE.QPwC84m4dy0vnY8X90ILnQ}
pwn.college{mqgYkkZOom8cjzXEtWGRriYb2dHK4qPHMRXZl713wMsLu2H}
pwn.college{gzlM8ibC9ILrmytFXutpvaWDXMQudTdOKoYAakHLomsz0Ep}
pwn.college{AYxr258ZSywtQToW25PLJ6RZwgM6rO4VbyvHZ8PlaIxzXb0}
pwn.college{J5lOhAgniaLF79-YCynB8bGPuu6Lvga-7yISLdP1zXiSWsk}
pwn.college{BxFDv3bsOWUv5yJV0kJVdMQKUrJPwgf38CsOvbPZQINBHqg}
pwn.college{PtSLMpU7KxdrTiA1J5Axtsn9xlzvgxW1IbE6UYTCFEOgTQI}
pwn.college{lPo0MOjskTzsv.9HTgKu0E1AELvVZf5S4J6D01DReJW3PdN}
pwn.college{j-VzzY2LK01NveZUU9LMaypx-6nVujmL8AGUGEzqtHWVyfW}
pwn.college{pSv0vdBoHv.Ux1c7.cejiVkXEy48-STZHh5adP22VVMPPw7}
pwn.college{M6kqt-2jtT7FM1YKRXlXbhR3mNzDb6K-TCdTf.K9ys-ssXX}
pwn.college{njs65FIyXS5RRTMjEnW26AriMx3HvQyECj5WKOMl-0jHQQX}
pwn.college{hhT.jluQIZm443nwkPkVAnYT7zAvCJSEynvsO65AswP6fvW}
pwn.college{-W.WnzIM-MwXrzP8ok3nUq4QhR8VenMdLz-F5-gYRQ1qex9}
pwn.college{ac9xlqwZZ5rNXdBZ9WGHvmgPbPmU6CyWDGWsw95YEeXTkHp}
pwn.college{UrTPb2e-N0YQmGWtwmC20HV6Dpf9BJQbbfpySZscWoaP5T-}
pwn.college{FcdD4TyO2jP7sgoFehBQxnmJVN6gpZwgXC0wLP6cMp1SXDt}
pwn.college{e0dpTSnhuPQ732G-nUaQ7mxynNMSKlk.E6rKvsbI8RCf28G}
pwn.college{bjqx1g-47bkDC1nEO6c-mAp10N.xliIKvf.BGSoqNSrrjqF}
pwn.college{vGd2Co2IPnJQOqscyXa1JhPITRJoB9OJUFcyLfG-uaqJwab}
pwn.college{0hwmaKsjcp6R-2JVY86kCpw9FuvuqJah1sxxyLZj3Qr-Z6g}
pwn.college{mmq63zk1IqWV2MQ8FwBTmAbcHhkJVy6F6ArN7toJ0tGqLVV}
pwn.college{7ZyHzy9xB5VHE0K-JjAEUw5yHfWiiRe4qHV8UrJ7eHncSUx}
pwn.college{LWUylXWgtqkzW5isgue-YV3WUKpo-6RlbC1PJ77E4K3ph4W}
pwn.college{PZ1gmFUUUkQoD6fXyKtGI96ZHb9xJ3GtGKQVHApLSzA8kYd}
pwn.college{Z1KDEbVuFMrVnhwmK9Gi5Wa7FJyIF1wMKl.YC8sgb6PUb-z}
pwn.college{AcV69Dz02nt5lBrvbeJnT5pQgpdlb0qLzPaX35qu17xrie2}
pwn.college{GpRuYr9wXkNqowNZXdNS.DL8XrhqSXcjCv-GbQ-ZFkfC26i}
pwn.college{dHVSZvrhgeKORTsnV698bgSi4ASfLh33T.yhVebaVS1HpLm}
pwn.college{dMNrdiW8-SXzGqUnxFQbJtlp2LdfV2NgxcDON1INLbwKTHC}
pwn.college{I.87B9vY-Kr.Z0tbPlf.AFSmb2I01TDqsKsmdC6SVqgmtmt}
pwn.college{6VaWlmHQLwrjnFAaEPKjTzrJoVK3KdD.CcpvEbzW-DOcdZ6}
pwn.college{J7A-mH-4HIoW6bTq90SXyEG1x3AJG9Ka3qEAxgQZXKe.9Gv}
pwn.college{xZ-CjYFOGXvBeINlAsyMjV4fR1GhLVYbTTWHEvC91btYtb4}
pwn.college{C45cA6pj5auu7mCJe4QxDdvSXRCOWyQm05ANQVpYuDOX.dw}
pwn.college{1oJMO.WdUJi0ikLtcDGzP-L9igXRXSc9OgmbIK6qdoYr3hk}
pwn.college{fz1LxkFyjp3anHJcmyPfKmgvSHIXtedwzjn3N8TXaXiI9td}
pwn.college{5jVBH5x25CwC53ZiQjq5c1CQL2YEj7Udi3YUZfFwFOxeX1D}
pwn.college{IpokTP0A2fbbUc9LSKkXBxYFN6FHBSMfUdrMu--XqZj7-0q}
pwn.college{zbWq173H0uJj-7xGQ2Qb6hFUhUEU1hq-3N88GGcaKdQC6cj}
pwn.college{4m13ooQXLHk0cA8qQA5fbmN6UzBNI-Sx.UQwev7KswLa9F6}
pwn.college{TOC7amReBbOZfELkenliTEPbc7Me-0ltdRg0U4VCo6YugkB}
pwn.college{0FhjuN3uI3Fzq1.BvuUwyCnRo5AAmjZphn4hRZTEyVWdDaR}
pwn.college{ra4lLa08BBwioVl9bdNcx5co4OAoWLv04lTCDdPMX1EKma5}
pwn.college{xenmF3-wthpI-pr2dPtqEFe-dTi3UzAKoKrMrC86Odw8aa5}
pwn.college{Q9pFpgDOG2QCinV85uHMuGVJrWawYRpfLYJusHNnf7gjzsb}
pwn.college{.vCGkqcLwrjiSW4OgBtRYt8jRjRfGz9f3ITj1PJVO1XQA3W}
pwn.college{V7WGIJmdPAFNLVCyaeFQzh4bDF6CiX2hzi6L3NS3RuJ52gX}
pwn.college{DUmkT7l2Ie.IUUaT1UlGXFtvL4KmzgdzOAeACdOd5O5lj19}
pwn.college{9KZsG5g5qG.vYeRG8zkUXBz2zG5TCTnnRDs6m0DLtjGnxvK}
pwn.college{.L7IAPDgK7TW6uvMQJdbGiJUuCi8mN4R4w61MhK.YM7MCF.}
pwn.college{.dtCP6sAxmcb8WjpPm68ZX38lYM7zxYFkePAU2c3I.Wvj0X}
pwn.college{ujZXV04IcZe.e6MEGrCZX35WxQhHKhjcz5o5yNWQqequ3-f}
pwn.college{McZ.JwHDtm5bf5dqWBlK807WTw4F.lSIzAfqVbuUJCS5Bon}
pwn.college{Oe2Yyfj-J4fjI5jl0QT7w4bkG4rYOu1lfqR3Ohp0-CyD5dW}
pwn.college{UjLg0.KMfJSPdFflD8RWT3YzGKdyAxh9xWk70oBHnO74C5o}
pwn.college{54yk2OwckWnJ5QvSCbR4NUxwQkB5iwYmBi4ErjPYeCV2UJI}
pwn.college{R71g6xADxZ-yf9SBAPnYYSLDS4soggMRgEsQbZBnRyx2tTu}
pwn.college{75beQHFeh1TWa0guSz00.xYR27DPz9wygl02appROI2J1Yc}
pwn.college{3gEVBJj4CTSDgJKR1KOyyLYjyBkCMD20f..iDwz9e02cdLT}
pwn.college{3yV1.paXIhHHKeRdJXK0RXVkaFDQed.fhmbPznB.77EIbyB}
pwn.college{R7d3EZz64UOwlLliod--pXpFUeSBtbmJR4zf4YO0kbVKr9r}
pwn.college{ki3xcYSORiUH7YtJ-39v0fL8Be3HfhPK0BdRzfazoc.0oHp}
pwn.college{mSJG2YPYsT.pQu9.1dMaw2wMuSaXkY96aIQVyi.1haC6-TW}
pwn.college{AvtnOOFIB8pwdtLOXsX95_qfoL8.0FNzMDOxwSO1EzNzEzW}
pwn.college{AvtnOOFIB8pwdtLOXsX95_qfoL8.0FNzMDOxwSO1EzNzEzW}
```

## What I Learned
Learned how to kill files in fifo system

## References
None