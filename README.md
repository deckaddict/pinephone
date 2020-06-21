Any notes on how to make the pinephone work to get the tasks done.

To start bluetooth upon boot on alpine images
sudo cp startbt.start to /etc/local.d/

export current keymap: 'xkbcomp $DISPLAY def.xkb'
set new keymap: 'xkbcomp -Ipath/to/xkbfile/directory path/to/xkbfile $DISPLAY'

