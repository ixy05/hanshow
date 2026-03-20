# Hanshow


## Initial Wiring
| EPaper Tag | UART Flasher |
| --- | --- |
| GND | GND |
| VCC* | 3v |
| SWS | TXD |
| NRST | DTR^ |

\* only needed if battery is disconnected

\^ DTR pin is not made availible to all UART programmers. You may need to manually solder from the UART chip itself.

## Flashing
1. Wire as per table above
1. Go to [ATC_BLE_OEPL Uploader](https://atc1441.github.io/ATC_BLE_OEPL_Image_Upload.html)
2. Open **USB-COM** (must be done in Edge/Chrome)
3. Leave Baud and Activiation as they are
4. Optional: Set Device Type. This depends on your display. This can be changed later.
5. 'Load ATC_BLE_OEPL.bin'
6. 'Write Firmware', if you set a Device Type (from step 4), click 'Write Firmware and Type'
7. You know it will be working as the LED will be flashing. If not, check your wiring

### UART Flasher
I was able to use an ESP-01 programmer to flash my EPaper displays. I had to solder a wire to connect DTR pin on the CH340 to the epaper display.

### Confirmed Tag Types
1. Nebular 350R-N
2. Nebular 346

## Video Tutorial
https://youtu.be/9oKWkHGI-Yk

## Tools
| Tool | Link |
| --- | --- | --- | --- |
| BLE + Serial OEPL Uploader + Controller | [ATC_BLE_OEPL Uploader](https://atc1441.github.io/ATC_BLE_OEPL_Image_Upload.html) |


## Attributions
- https://github.com/atc1441/ATC_TLSR_Paper
- https://github.com/garobcsi/ATC_TLSR_Paper
- https://github.com/dontrajik/Nebular 
