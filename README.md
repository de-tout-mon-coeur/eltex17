Задание 1.
1. make defconfig
2. make menuconfig
3. make bzImage
4. make modules
5. sudo make modules_install
6. sudo make install

Задание 2.
1. ARCH=arm make defconfig
2. ARCH=arm make menuconfig
3. ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- make -j 4 zImage
4. ARCH=arm make -j 4 dtbs
5. QEMU_AUDIO_DRV=none qemu-system-arm -M vexpress-a9 -kernel zImage -dtb vexpress-v2p-ca9.dtb -append "console=ttyAMA0" -nographic
