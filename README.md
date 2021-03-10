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

Follow the instructions in [Getting started with Raspberry Pi Pico](https://datasheets.raspberrypi.org/pico/getting-started-with-pico.pdf) to install the Raspberry Pi Pico SDK. Then run the following:

```
mkdir build
cd build
cmake ..
make
```
