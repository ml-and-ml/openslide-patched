## Patch
Base `openslide` has a memory leak due to file cacheing. This version stores no cache and thus large amounts of slides can be loaded and reloaded without worry of depleting memory.

## OpenSlide

Carnegie Mellon University and others
https://openslide.org/

## How to build?

Install `autoconf, automake, libtool, and pkg-config` using pip<br/>
`autoreconf -i`<br/>
`./configure`<br/>
`make`<br/>
`make install`<br/>

Update paths:

`export PATH=/${HOME}/*/bin:/${HOME}/*/lib:$PATH`<br/>
`export LD_LIBRARY_PATH=/${HOME}/*/lib:$LD_LIBRARY_PATH`<br/>
`export LIBRARY_PATH=/${HOME}/*/lib:$LIBRARY_PATH`

