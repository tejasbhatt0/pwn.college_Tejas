# An Epic Filesystem Quest
In this challenge we put to use out combined knowledge of "cd", "ls" and "cat".

## My solve
**Flag:** `pwn.college{YXoAIcPSzN0kj6Hc_qOBdZj8cl9.QX5IDO0wiN2gjNzEzW}`

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
BRIEF  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin    challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat BRIEF
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/Documentation/livepatch

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.5/Documentation/livepatch
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.4/Documentation/livepatch
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/livepatch$ ls
MEMO  callbacks.rst  cumulative-patches.rst  index.rst  livepatch.rst  module-elf-format.rst  shadow-vars.rst
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/livepatch$ cat MEMO
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/media/pci
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/livepatch$ cd /opt/linux/linux-5.4/drivers/media/pci
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/media/pci$ ls
BLUEPRINT  b2c2        cobalt   cx25821   dm1105  ivtv    netup_unidvb  pt1      saa7146  solo6x10  tw5864
Kconfig    bt8xx       cx18     cx88      dt3155  mantis  ngene         pt3      saa7164  sta2x11   tw68
Makefile   built-in.a  cx23885  ddbridge  intel   meye    pluto2        saa7134  smipcie  ttpci     tw686x
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/media/pci$ cat BLUEPRINT
Congratulations, you found the clue!
The next clue is in: /usr/include/atomic_ops/sysdeps/ibmc

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/media/pci$ cd /usr/include/atomic_ops/sysdeps/ibmc
hacker@commands~an-epic-filesystem-quest:/usr/include/atomic_ops/sysdeps/ibmc$ ls
CUE  powerpc.h
hacker@commands~an-epic-filesystem-quest:/usr/include/atomic_ops/sysdeps/ibmc$ cat CUE
Lucky listing!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/hwclock

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/include/atomic_ops/sysdeps/ibmc$ ls /opt/busybox/busybox-1.33.2/include/config/feature/hwclock
INFO-TRAPPED  adjtime
hacker@commands~an-epic-filesystem-quest:/usr/include/atomic_ops/sysdeps/ibmc$ cat /opt/busybox/busybox-1.33.2/include/config/feature/hwclock/INFO-TRAPPED
Yahaha, you found me!
The next clue is in: /usr/share/doc/libselinux1-dev
hacker@commands~an-epic-filesystem-quest:/usr/include/atomic_ops/sysdeps/ibmc$ cd /usr/share/doc/libselinux1-dev
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libselinux1-dev$ ls
GIST  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libselinux1-dev$ cat GIST
Tubular find!
The next clue is in: /opt/pwn.college/vm

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libselinux1-dev$ cd /opt/pwn.college/vm
hacker@commands~an-epic-filesystem-quest:/opt/pwn.college/vm$ ls -a
.  ..  .SNIPPET  init  vm
hacker@commands~an-epic-filesystem-quest:/opt/pwn.college/vm$ cat .SNIPPET
Congratulations, you found the clue!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/ash/optimize/for

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/pwn.college/vm$ cd /opt/busybox/busybox-1.33.2/include/config/ash/optimize/for
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/ash/optimize/for$ ls -a
.  ..  .CLUE  size.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/ash/optimize/for$ cat .CLUE
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/include/config/oprofile/nmi

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/ash/optimize/for$ cd /opt/linux/linux-5.4/include/config/oprofile/nmi
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/oprofile/nmi$ ls
SPOILER  timer.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/config/oprofile/nmi$ cat SPOILER
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{YXoAIcPSzN0kj6Hc_qOBdZj8cl9.QX5IDO0wiN2gjNzEzW}
```

## What I learned
N.A.

## Incorrect tangents
N.A.

## References
N.A.
