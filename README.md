[M681-intl](http://www.meizu.com)
=================

M681 repo is Linux kernel source code for Meizu M3 Note International smartphones. With this repo, you can customize the source code and compile a Linux kernel image yourself. Enjoy it!

HOW TO COMPILE
-----------

###1. Download source code###

  <code>git clone https://github.com/meizuosc/m681-intl.git</code>

###2. Compiling###

```
mkdir out
make ARCH=arm64 CROSS_COMPILE=aarch64-linux-android- O=`pwd`/out m3note_intl_defconfig
make -j8 ARCH=arm64 CROSS_COMPILE=aarch64-linux-android- O=`pwd`/out
```

  Note:
  + Make sure you have arm cross tool chain, maybe you can download [here](http://www.linaro.org/downloads)
  + If you get a poor cpu in your compiling host, you should use "-j4" or lower instead of "-j8"

Get Help
--------

Checkout our community http://bbs.meizu.cn (in Chinese)
