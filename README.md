# linux-5.7.6
基于JZ2440的linux-5.7.6内核移植
使用交叉编译工具链gcc version 8.3.0 (crosstool-NG 1.24.0)

特性：
1.支持uboot传入的machid为MACH_TYPE_S3C2440，对应smdk2440单板，其值为362，16进制0x16A。
2.支持uboot传入的machid为MACH_TYPE_MINI2440，对应mini2440单板，其值为1999，16进制0x7CF（MINI2440预设的device更为丰富，smdk2440暂未设置device_eth，需要修改smdk2440_devices数组）。
3.支持yaffs2,jffs2文件系统。

编译方法：
1.make jz2440_defconfig或者make menuconfig自定义
2.make uImage

