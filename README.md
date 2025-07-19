# Kai Cosmos 40, a ZMK split keyboard with pmw3610 trackball

Design is mostly created using [rianadon's Cosmos Keyboard Configurator](https://github.com/rianadon/Cosmos-Keyboards). Highly recommend! It's a godsend.

What I did:
1. Scan my own hands with the tools Cosmos Keyboard Configurator provided and my phone's camera.
2. Add a 34mm trackball with Skree ZMK to the right side, which will also be ZMK's main side.
3. Download the models and edit in Blender and Fusion to smooth the corners.
4. Using the microcontroller holder template from Cosmos Keyboard Configurator, draw out PCB in Kicad.
5. Implement [badjeff's zmk-pmw3610-driver](https://github.com/badjeff/zmk-pmw3610-driver/tree/main) with some official ZMK settings. Documentations aren't really clear, I recommend searching and copying from public repos on Github.
6. Solder, test, rinse and repeat.

Things for further improvements:
1. Reset button should be set under MCU holder PCB for easier access.
2. Should have cutouts under MCUs to make built-in LEDs more visible.