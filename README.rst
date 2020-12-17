===========
QEMU-RASPINLOOP README
===========
Fork of QEMU for use with raspinloop Project.
QEMU is a generic and open source machine & userspace emulator and
virtualizer. This fork exchange raspi3 GPIO state with a backend service named ria-cosimulation-worker ( via ria-proxy-server). 

QEMU as a whole is released under the GNU General Public License,
version 2. For full licensing details, consult the LICENSE file.


Building
========

QEMU is multi-platform software intended to be buildable on all modern
Linux platforms, OS-X, Win32 (via the Mingw64 toolchain) and a variety
of other UNIX targets. 

The steps to build this version of QEMU are:


.. code-block:: shell

  mkdir build
  cd build
  ../configure --target-list=aarch64-softmmu,aarch64-linux-user --enable-zmq
  make

