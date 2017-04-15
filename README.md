# i386-elf-toolchain PKGBUILDs

This repository contains the PKGBUILD recipes for building a few tools required
for building, running and testing i386-elf-binaries such as 32 bit operating
system kernels based on the ELF format, like NativeOS - although it may suit to
build and test other kernels.

At the moment this repository has been tested successfully on Arch Linux. It
should work on other Arch-based distributions as well such as Manjaro. There
is interest on testing and porting these scripts on MSYS2 for Windows, which
also makes use of the pacman package manager, in order to have builds for
Windows (MSYS target only) as well.

## How to install

Change directory to the package to be built. There should be a PKGBUILD on
your current directory. Run `makepkg`.

    $ cd pkgbuild-i386-elf-toolchain/i386-elf-binutils
    $ makepkg

You will get a package. Something something _<pkgname>.pkg.tar.xz_. Run
`pacman -U <pkgname>.pkg.tar.xz` to install it.

Please, refer to the docs if you need more help:

* https://wiki.archlinux.org/index.php/makepkg
* https://wiki.archlinux.org/index.php/pacman
