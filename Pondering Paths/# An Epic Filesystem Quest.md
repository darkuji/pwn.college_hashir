# An Epic Filesystem Quest
### The challenge asks us to check various directories using the commands we know to find clues for the flag


## My Solve
**Flag:** pwn.college{4DlilFxlUAASbEumEBZDGSIItcZ.QX5IDO0wSO1EzNzEzW}
I first used the ls command to get the name of the file with the first clue
and used the cat command to read it. The next file was supposed to be hidden
so i used ls -a along with the file path to get its name followed by the cat
command to read it. The next file was trapped so i used cat along with its 
absolute path instead of changing my cwd. The next 2 clues were normal so i used
ls and cat to fetch them. The clue after it was trapped meaning I had to cat it
using its absolute path. The clue after that was delayed meaning I had to change
my cwd to its folder before having to cat it. The last clue was a regular one so 
I just had to ls and cat it to obtain the flag. 


```
hacker@commands~an-epic-filesystem-quest:/$ ls
TEASER  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin     challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat TEASER
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/include/config/hid

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/linux/linux-5.4/include/config/hid -a
.        a4tech.h  cherry.h   ezkey.h     ite.h         microsoft.h  pantherlord.h  redragon.h  sunplus.h
..       apple.h   chicony.h  generic.h   kensington.h  monterey.h   petalynx.h     samsung.h   topseed.h
.NUGGET  belkin.h  cypress.h  gyration.h  logitech.h    ntrig.h      pid.h          sony.h
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/linux/linux-5.4/include/config/hid/.NUGGET
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/IPython/core/tests

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/lib/python3/dist-packages/IPython/core/tests
2x2.jpg         simpleerr.py           test_displayhook.py        test_inputtransformer2_line.py  test_profile.py
2x2.png         tclass.py              test_events.py             test_interactiveshell.py        test_prompts.py
NOTE-TRAPPED    test_alias.py          test_extension.py          test_iplib.py                   test_pylabtools.py
__init__.py     test_application.py    test_formatters.py         test_logger.py                  test_run.py
__pycache__     test_async_helpers.py  test_handlers.py           test_magic.py                   test_shellapp.py
bad_all.py      test_autocall.py       test_history.py            test_magic_arguments.py         test_splitinput.py
daft_extension  test_compilerop.py     test_hooks.py              test_magic_terminal.py          test_ultratb.py
nonascii.py     test_completer.py      test_imports.py            test_oinspect.py
nonascii2.py    test_completerlib.py   test_inputsplitter.py      test_page.py
print_argv.py   test_debugger.py       test_inputtransformer.py   test_paths.py
refbug.py       test_display.py        test_inputtransformer2.py  test_prefilter.py
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/python3/dist-packages/IPython/core/tests/NOTE-TRAPPED
Great sleuthing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/pythonjsonlogger
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/local/lib/python3.8/dist-packages/pythonjsonlogger
SECRET       __pycache__  defaults.py   json.py        msgspec.py  py.typed
__init__.py  core.py      exception.py  jsonlogger.py  orjson.py   utils.py
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/local/lib/python3.8/dist-packages/pythonjsonlogger/SECRET
Lucky listing!
The next clue is in: /opt/pwndbg/docs/commands/xinfo
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/pwndbg/docs/commands/xinfo
TRACE  xinfo.md
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/pwndbg/docs/commands/xinfo/TRACE
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/sage/schemes

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls  /usr/lib/python3/dist-packages/sage/schemes
TIP-TRAPPED  affine  cyclic_covers    hyperelliptic_curves  plane_quartics      readme.py
__init__.py  all.py  elliptic_curves  jacobians             product_projective  riemann_surfaces
__pycache__  curves  generic          plane_conics          projective          toric
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/python3/dist-packages/sage/schemes/TIP-TRAPPED
Yahaha, you found me!
The next clue is in: /usr/lib/python3/dist-packages/dateutil/parser

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/lib/python3/dist-packages/dateutil/parser -a
.  ..  .BLUEPRINT  __init__.py  __pycache__  _parser.py  isoparser.py
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/python3/dist-packages/dateutil/parser/.BLUEPRINT
Congratulations, you found the clue!
The next clue is in: /usr/share/locale/mr

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/locale/mr
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/mr$ ls
LC_MESSAGES  POINTER
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/mr$ cat POINTER
Lucky listing!
The next clue is in: /usr/lib/x86_64-linux-gnu/perl-base/unicore/lib/CWL

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/locale/mr$ cd /usr/lib/x86_64-linux-gnu/perl-base/unicore/lib/CWL
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl-base/unicore/lib/CWL$ ls
HINT  Y.pl
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl-base/unicore/lib/CWL$ cat HINT
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{4DlilFxlUAASbEumEBZDGSIItcZ.QX5IDO0wSO1EzNzEzW}
```

## What I Learned
I learned how different types of files need different ways of searching like for example
hidden files need -a, delayed files need for us to change the cwd and other methods.

## References
None 