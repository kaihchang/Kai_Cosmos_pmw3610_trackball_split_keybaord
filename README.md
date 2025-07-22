# Kai Cosmos 40, a ZMK split keyboard with pmw3610 trackball

[👉 ZMK firmware](https://github.com/kaihchang/zmk-config-kai-cosmos)

![PXL_20250718_123022295](https://github.com/user-attachments/assets/a8bea65b-cee5-49db-9836-d94d528a0886)
![PXL_20250719_032243330](https://github.com/user-attachments/assets/1e5e8041-8a9d-499b-8874-9932b3508b27)
![PXL_20250719_032322315](https://github.com/user-attachments/assets/c7f91561-b00e-41f1-843d-26ff90888ce5)
![PXL_20250719_032409798](https://github.com/user-attachments/assets/88b3f06e-d8a6-4f64-bc1d-f5604646f808)

Design is mostly created using [rianadon's Cosmos Keyboard Configurator](https://github.com/rianadon/Cosmos-Keyboards). Highly recommend! It's a godsend.

What I did:
1. Scan my own hands with the tools Cosmos Keyboard Configurator provided and my phone's camera.
2. Add a 34mm trackball with [Skree ZMK pmw3610 board](https://github.com/siderakb/pmw3610-pcb) to the right side, which will also be ZMK's main side.
3. Download the models and edit in Blender and Fusion to smooth out the corners.
4. Using the microcontroller template from Cosmos Keyboard Configurator to draw out PCB in Kicad.
5. Implement [badjeff's zmk-pmw3610-driver](https://github.com/badjeff/zmk-pmw3610-driver/tree/main) with some official ZMK settings. Documentations aren't really clear, I recommend searching certain attributes and copying from public repos on Github.
6. Solder, test, change keymap, rinse and repeat.
<img width="1489" height="615" alt="cosmos_configurator" src="https://github.com/user-attachments/assets/b41d1a4b-21b9-4ec6-947d-7a9dced39dc8" />
<img width="1332" height="1125" alt="mcu_holder" src="https://github.com/user-attachments/assets/026d34c9-2e1e-4e79-93a0-0e0932c19253" />

Things for further improvements:
1. Reset button should be set under MCU holder PCB for easier access.
2. Should have cutouts under MCUs to make built-in LEDs more visible.
3. Should have copper keep out zones beneath MCU's antennae for better Bluetooth signal.
4. Not crucial but important, pmw3610 orientation does matter, since with official settings you can only rotate it in 90-degree increments. Fortunately worked out for me, but I didn't know this beforehand.
