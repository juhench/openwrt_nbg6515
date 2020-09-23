# openwrt_nbg6515
OpenWrt Development Instructions for ZyXEL NBG6515 Router

The instructions are located here:
https://openwrt.org/toh/zyxel/zyxel_nbg6515_ac750

The 512 bytes patch and two tested downloads are included here, originally developed for the Ralink MT7620a + MT7530 evaluation board.

It is currently not possible to revert the router to the original firmware. It is therefore advisable to preserve the original firmware through TFTP booting OpenWrt and then saving the contents of the flash memory somewhere. Follow the detailed instructions on the OpenWrt project page. I am not responsible if you damage or brick your device. I have tried the instructions repeatedly and TFTP booting remains available. U-Boot is not modified during the procedures described.
