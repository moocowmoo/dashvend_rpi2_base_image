# dashvend_rpi2_base_image
'raspbian lite' raspberry pi 2 image configured for 480x800 lcd

# install

Find your sdcard address by looking at the end of the output of 'dmesg' after plugging in your sd card.
Do not use a partition number like 'sdb1', use the whole drive identifier 'sdb' (yours may be sda or sdc)
This command will destroy any data on the sd card. Use with caution.

    # be careful with this command, you can destroy data if you don't set the dd target (sd card location) correctly
    xzcat dashvend_base_image.img.xz | sudo dd of=/dev/sdb

