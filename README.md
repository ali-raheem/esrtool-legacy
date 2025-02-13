# esrtool v0.25.3

**This is tool is archived. Try this tool instead [esrtool_rs](https://github.com/ali-raheem/esrtool_rs/)**

A simple esr (un)patching tool.

Fork from 0.24a esr-disc-patcher-cli v0.24

Original thread: http://psx-scene.com/forums/f164/esr-disc-patcher-linux-mac-qt4-port-60096/

Mirror: https://web.archive.org/web/20150919031500/http://psx-scene.com/forums/f164/esr-disc-patcher-linux-mac-qt4-port-60096/

### Binaries

Statically linked stripped binary in /bin/

Functionally tested on:

* Windows 10
* Windows 10 WSL (should be linux compatible)

### Installation

Copy compiled binary (or provided statically linked one) to a folder in your path.

### Running

To apply ESR patch

```
$ ./esrtool p path_to_iso
```

To remove ESR patch

```
$ ./esrtool u patch_to_patched_iso
```

### Compilation

```
$ make
```

For the static binaries

```
$ make static
```

For windows rename esrtool.c esrtool.cpp and use Visual Studio C++.

### Todo

* Option to not patch in place

### Changelog
* 2022-01-21 Crash fix.
* 2017-05-11 Rewrite of interface code in c. Now esrtool.
* 2017-05-11 Added static make rules
* 2017-05-01 defines.h uses <csting> type includes
* 2017-04-30 forked from https://github.com/antipatico/esr-disc-patcher-cli
