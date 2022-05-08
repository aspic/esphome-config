# esphome configs

Collection of [esphome](https://esphome.io/) configs for various use-cases. These are calibriated for my devices/senors and probably need some tweaking if you copy/paste.

## Install over usb

First build the image with esphome, then install manually over USB. Typically when first setting up the device. First install esptool, then:

    esptool write_flash -fm dio 0x00000 ./custom-image.bin 

Defaults to `/dev/ttyUSB0`
