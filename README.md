# openwrt_nbg6515
OpenWrt Development Instructions for ZyXEL NBG6515 Router

The instructions are located here:
https://openwrt.org/toh/zyxel/nbg6515_ac750

The 512 bytes patch and two tested downloads are included here, originally developed for the Ralink MT7620a + MT7530 evaluation board.

It is currently not possible to revert the router to the original firmware. It is therefore advisable to preserve the original firmware through TFTP booting OpenWrt and then saving the contents of the flash memory somewhere. Follow the detailed instructions on the OpenWrt project page. I am not responsible if you damage or brick your device. I have tried the instructions repeatedly and TFTP booting remains available. U-Boot is not modified during the procedures described.

In case you have deleted the original firmware already, you can use the 512 bytes-sized file "soc_wmac.eeprom" and copy it into the location "/lib/firmware/soc_wmac.eeprom".

The images were downloaded 2020-09-23 and are working. Other releases are likely to work as well.
https://downloads.openwrt.org/releases/19.07.4/targets/ramips/mt7620/openwrt-19.07.4-ramips-mt7620-mt7620a_mt7530-initramfs-kernel.bin (for initial boot via TFTP)
https://downloads.openwrt.org/releases/19.07.4/targets/ramips/mt7620/openwrt-19.07.4-ramips-mt7620-mt7620a_mt7530-squashfs-sysupgrade.bin (to be flashed from LuCi after the device has booted successfully from TFTP).
