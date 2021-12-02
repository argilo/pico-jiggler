Mouse Jiggler for Raspberry Pi Pico
===================================

This program turns the Raspberry Pi Pico into a simulated mouse that periodically moves a small amount. This can be used to prevent screensavers from triggering.

Installation
------------

1. Download `jiggler.uf2` from the [latest release](https://github.com/argilo/pico-jiggler/releases/latest).
2. Plug in the Raspberry Pi Pico while holding the "BOOTSEL" button.
3. Drag the `jiggler.uf2` file into the "RPI-RP2" USB mass storage device that appears.

Building from source
--------------------

Clone repo and initialize pico-sdk, tinyusb submodules:
```
git clone https://github.com/akhilharihar/pico-jiggler.git && cd pico-jiggler
git submodule update --init
cd lib/pico-sdk && git submodule update --init
```

Then run the following:

```
mkdir build
cd build
cmake ..
make -j $nproc
```
