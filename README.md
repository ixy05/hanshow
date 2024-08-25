# Hanshow


## Wiring
| EPaper Tag | Flasher |
| --- | --- |
| GND | GND |
| VCC | 3v |
| SWS | TXD |
| NRST | GND |

## Flashing
1. Clone / [download repo ](https://github.com/atc1441/ATC_TLSR_Paper)
2. Baud: 460800, Atime: 3 sec
3. Open **USB-COM** (must be done in Edge/Chrome)
4. **Unlock flash** 
5. Select and upload firmware by **Choosing File**
6. **Write to flash**
7. ❗While "Activate (3 sec)" is on (and blue light is on EPaper), **disconnect** NRST from ground ❗


### Flasher
I was able to use an ESP-01 programmer to flash my EPaper displays. 

## Tools
| Tool | Usage | Compatability* | Link |
| --- | --- | --- | --- |
| UART Uploader | To upload '.bin' files to the epaper tags | All | https://atc1441.github.io/ATC_TLSR_Paper_UART_Flasher.html |
| Bluetooth Image Upload | Send a hex sequence to tag | [ATC_TLSR_Paper](https://github.com/atc1441/ATC_TLSR_Paper) | https://atc1441.github.io/ATC_TLSR_Paper_Image_Upload.html |
| Bluetooth OTA Uploader | Upload firmware; read RAM and flash storage; send CMDs | [ATC_TLSR_Paper](https://github.com/atc1441/ATC_TLSR_Paper) | https://atc1441.github.io/ATC_TLSR_Paper_OTA_writing.html |
| Bluetooth Controller | Send commands; upload images; upload drawings (made on web); clear screen | Primarily for [garobcsi/ATC_TLSR_Paper](https://github.com/garobcsi/ATC_TLSR_Paper) | https://garobcsi.github.io/ATC_TLSR_Paper/web_tools/ |

\* Compatability is not limited to what has been listed



## Attributions
- https://github.com/atc1441/ATC_TLSR_Paper
- https://github.com/garobcsi/ATC_TLSR_Paper
- https://github.com/dontrajik/Nebular 
