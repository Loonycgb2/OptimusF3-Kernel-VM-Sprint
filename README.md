OptimusF3-Kernel-VM-Sprint
==========================

Virgin Mobile &amp; Sprint Stock kernel source

Kernel Build
  - Unzip LS720_JB_kernel.tar.gz at the android folder
  - When you compile the kernel source code, you have to add google original prebuilt source(toolchain) 
     into the android folder.
    $ source ./build/envsetup.sh
    $ choosecombo 1 generic user
  - Build kernel
    $ cd Kernel
    $ make fx3_spcs_defconfig  ARCH=arm CROSS_COMPILE=arm-eabi-
    $ make ARCH=arm CROSS_COMPILE=arm-eabi-
  - After Build, You Can find the build image at arch/arm/boot
