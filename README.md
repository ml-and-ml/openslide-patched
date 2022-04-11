## Patch
Base `openslide` has a memory leak due to file cacheing. This version stores no cache and thus large amounts of slides can be loaded and reloaded without worry of depleting memory.

## OpenSlide

Carnegie Mellon University and others
https://openslide.org/

## How to build?

Install `autoconf, automake, libtool, and pkg-config` using pip
`autoreconf -i`
`./configure`
`make`
`make install`

Update paths:

`export PATH=/${HOME}/*/bin:/${HOME}/*/lib:$PATH`
`export LD_LIBRARY_PATH=/${HOME}/*/lib:$LD_LIBRARY_PATH`
`export LIBRARY_PATH=/${HOME}/*/lib:$LIBRARY_PATH`

