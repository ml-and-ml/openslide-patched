## Patch
Base OpenSlide has a memory leak due to file cacheing. This version stores no cache and thus large amounts of slides can be loaded and reloaded without worry of depleting memory.

OpenSlide

Carnegie Mellon University and others

https://openslide.org/


=======================


How to build?
=============

./configure
make
make install

(If building from the Git repository, you will first need to install
autoconf, automake, libtool, and pkg-config and run "autoreconf -i".)

Update paths:


export PATH=/home/user/temp-install/*/bin:/home/ec2-user/temp-install/openslide-3.4.1/lib:$PATH
export LD_LIBRARY_PATH=/home/user/*/openslide-3.4.1/lib:$LD_LIBRARY_PATH
export LIBRARY_PATH=/home/user/*/openslide-3.4.1/lib:$LIBRARY_PATH

