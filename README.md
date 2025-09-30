# M5Dial-LVGL

PIO + ESP-IDF + LVGL for M5Stack Dial

## Uses
- PlatformIO
- ESP-IDF **v5.1.2**.
- LVGL: **9.x**. Earlier LVGL versions are incompatible.

## Usage

Call `m5dial_lvgl_init()` first, `m5dial_lvgl_next()` in a loop.
Please refer to examples for more details.

## Examples

| [hello_world]| [touch_button]| [dial_number]|
|:------------:|:-------------:|:------------:|
|![hello-world]|![touch-button]|![dial-number]|
|Simple drawing|  Touch input  | Encoder input|

|  [qr_code]  |  [new_font] | [native_sdl]|
|:-----------:|:-----------:|:-----------:|
| ![qr-code]  | ![new-font] |![native-sdl]|
|Custom config|External font|  PC preview |

[hello_world]: ./examples/hello_world
[touch_button]: ./examples/touch_button
[dial_number]: ./examples/dial_number
[qr_code]: ./examples/qr_code
[new_font]: ./examples/new_font
[native_sdl]: ./examples/native_sdl

[hello-world]: ./examples/hello_world/preview.png
[touch-button]: ./examples/touch_button/preview.png
[dial-number]: ./examples/dial_number/preview.png
[qr-code]: ./examples/qr_code/preview.png
[new-font]: ./examples/new_font/preview.png
[native-sdl]: ./examples/native_sdl/preview.png

## Hardware

- Confirm SPI MOSI/MISO/SCLK, CS, DC, RST, BL and touch pins match your board. Update driver files if needed.

## License

- Project code: [MIT](LICENSE)

### Third-Party Notices
- LVGL v9: MIT — see https://github.com/lvgl/lvgl
- M5Unified: see upstream license (MIT) — https://github.com/m5stack/M5Unified
- ESP-IDF (toolchain/framework): Apache-2.0 — https://github.com/espressif/esp-idf
- FreeRTOS (via ESP-IDF): MIT — https://www.freertos.org
- SDL2 (native_sdl example only): zlib — https://www.libsdl.org
- Big Shoulders Stencil Display font (examples/new_font): SIL Open Font License 1.1 — https://fonts.google.com/specimen/Big+Shoulders+Stencil+Display
