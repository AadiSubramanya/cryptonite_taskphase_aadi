# Filesystem quest
## Code:
```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
SECRET  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin     challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat SECRET
Tubular find!
The next clue is in: /usr/share/icons/hicolor/128x128/categories

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd  /usr/share/icons/hicolor/128x128/categories
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/128x128/categories$ ls
DOSSIER
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/128x128/categories$ cat DOSSIER
Yahaha, you found me!
The next clue is in: /usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/128x128/categories$ /usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__
ssh-entrypoint: /usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/128x128/categories$ cd /usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__$ ls
CUE                      _build_latex_antlr.cpython-38.pyc  errors.cpython-38.pyc
__init__.cpython-38.pyc  _parse_latex_antlr.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__$ cat CUE
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/gi/overrides/__pycache__

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/sympy/parsing/latex/__pycache__$ cd /usr/lib/python3/dist-packages/gi/overrides/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ ls
EVIDENCE                           GObject.cpython-38.pyc    Gedit.cpython-38.pyc  Pango.cpython-38.pyc
GIMarshallingTests.cpython-38.pyc  Gdk.cpython-38.pyc        Gio.cpython-38.pyc    __init__.cpython-38.pyc
GLib.cpython-38.pyc                GdkPixbuf.cpython-38.pyc  Gtk.cpython-38.pyc    keysyms.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ cat EVIDENCE
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/include/nvkm/subdev/bios

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ cat /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/include/nvkm/subdev/bios
cat: /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/include/nvkm/subdev/bios: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ ls /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/include/nvkm/subdev/bios
DISPATCH-TRAPPED  P0260.h  conn.h   dp.h      i2c.h       mxm.h   pll.h           rammap.h  volt.h
M0203.h           bit.h    cstep.h  extdev.h  iccsense.h  npde.h  pmu.h           therm.h   vpstate.h
M0205.h           bmp.h    dcb.h    fan.h     image.h     pcir.h  power_budget.h  timing.h  xpio.h
M0209.h           boost.h  disp.h   gpio.h    init.h      perf.h  ramcfg.h        vmap.h
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ cat DISPATCH-TRAPPED
cat: DISPATCH-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ cat /opt/linux/linux-5.4/drivers/gpu/drm/nouveau/include/nvkm/subdev/bios/DISPATCH-TRAPPED
Tubular find!
The next clue is in: /opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/gi/overrides/__pycache__$ cd /opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads$
 ls -a
.  ..  .TRACE  master
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads$
 cat .TRACE
Lucky listing!
The next clue is in: /usr/lib/python3/dist-packages/IPython/core/__pycache__

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads$
 ls  /usr/lib/python3/dist-packages/IPython/core/__pycache__
SNIPPET-TRAPPED               display.cpython-38.pyc       hooks.cpython-38.pyc              payload.cpython-38.pyc
__init__.cpython-38.pyc       display_trap.cpython-38.pyc  inputsplitter.cpython-38.pyc      payloadpage.cpython-38.pyc
alias.cpython-38.pyc          displayhook.cpython-38.pyc   inputtransformer.cpython-38.pyc   prefilter.cpython-38.pyc
application.cpython-38.pyc    displaypub.cpython-38.pyc    inputtransformer2.cpython-38.pyc  profileapp.cpython-38.pyc
async_helpers.cpython-38.pyc  error.cpython-38.pyc         interactiveshell.cpython-38.pyc   profiledir.cpython-38.pyc
autocall.cpython-38.pyc       events.cpython-38.pyc        latex_symbols.cpython-38.pyc      prompts.cpython-38.pyc
builtin_trap.cpython-38.pyc   excolors.cpython-38.pyc      logger.cpython-38.pyc             pylabtools.cpython-38.pyc
compilerop.cpython-38.pyc     extensions.cpython-38.pyc    macro.cpython-38.pyc              release.cpython-38.pyc
completer.cpython-38.pyc      formatters.cpython-38.pyc    magic.cpython-38.pyc              shellapp.cpython-38.pyc
completerlib.cpython-38.pyc   getipython.cpython-38.pyc    magic_arguments.cpython-38.pyc    splitinput.cpython-38.pyc
crashhandler.cpython-38.pyc   history.cpython-38.pyc       oinspect.cpython-38.pyc           ultratb.cpython-38.pyc
debugger.cpython-38.pyc       historyapp.cpython-38.pyc    page.cpython-38.pyc               usage.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads$
 cat  /usr/lib/python3/dist-packages/IPython/core/__pycache__/SNIPPET-TRAPPED
Great sleuthing!
The next clue is in: /opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/cbindgen-236b0b4047138d63

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/QEMU-Nyx/modules/libxdc/logs/refs/heads$
 cd /opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/cbindgen-236b0b4047138d63
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/cbindgen-236b0b4047138d63$ ls -a
.  ..  .LEAD  build-script-build  build_script_build-236b0b4047138d63  build_script_build-236b0b4047138d63.d
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/cbindgen-236b0b4047138d63$ cat .LEAD
Lucky listing!
The next clue is in: /opt/aflplusplus/qemu_mode/qemuafl/include/hw/pci-bridge

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/nyx_mode/libnyx/libnyx/target/release/build/cbindgen-236b0b4047138d63$ cd  /opt/aflplusplus/qemu_mode/qemuafl/include/hw/pci-bridge
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/include/hw/pci-bridge$ ls -a
.  ..  .README  simba.h
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/include/hw/pci-bridge$ cat .README
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{ItEC5bJndRr-KRt5BNaQeJERUNx.dljM4QDLycjN0czW}
```
## Learnings:
Understanding commands and arguments

## References:
None
