Run the emulation with:

 qemu-system-ppc64 -M pseries -cpu POWER7 -m 256 -kernel output/images/vmlinux -append "console=hvc0 rootwait root=/dev/sda" -drive file=output/images/rootfs.ext2,if=scsi,index=0,format=raw -serial stdio -display curses

The login prompt will appear in the terminal that started Qemu.

Tested with QEMU 2.12.0
