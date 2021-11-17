# TG3442DE Teardown

A fun project disassembling and understanding a Vodafone TG3442DE cable router (aka `Arris Touchstone TG3442`: [commscope.com product page](https://www.commscope.com/product-type/broadband-video-devices/broadband-devices/docsis-3.1-gateways-modems/tg3442/)).

## Goals

1. Using the cable-interface for wiretapping and analyzing the DOCSIS 3.1 Protocol
2. Understanding why Vodafone does not support IPv6-addresses while the router is in bridge mode (to be proven: IPv6 is used for VoIP-Telephony and is therefore terminated at the TG3442 running in bridged mode)

## Hardware

For Hardware-Identification see: [Hardware.md](./Hardware.md)

| Information:               | Description:                                                                                                                                                                                                              |
| :------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Branding:                  | `Vodafone`                                                                                                                                                                                                                |
| Model No.:                 | `TG3442DE`                                                                                                                                                                                                                |
| Hardware Version:          | `MP1`                                                                                                                                                                                                                     |
| CPU:                       | `Intel FHCE2752M` (Intel Puma 7 SoC CE2752M) 2 cores, 2.5 GHz, Intel Atom Arch ([Intel Puma 7 product family page](https://ark.intel.com/content/www/de/de/ark/products/140087/intel-puma-7-family.html))                 |
| RAM:                       | `Samsung K4B2G1646F-BYK0` ???Capacity used (4x512 MByte?)??? 4x DDR3-RAM ([Samsung product page](https://www.samsung.com/semiconductor/dram/ddr3/K4B2G1646F-BYK0/)) [FIXME: exact capacity]                               |
| Flash:                     | `Kioxia TC58NVG2S0HBAI4` 512 MByte SLC NAND EEPROM (Toshiba/[Kioxia product page](https://business.kioxia.com/en-us/memory/detail.TC58NVG2S0HBAI4.html))                                                                  |
| Subscriber Line IC (SLIC): | `Microsemi ZL88107` Microsemi Corporation, ???maybe part of ZL880 series -> [product page](https://www.microchip.com/design-centers/interface-and-connectivity/line-circuits)??? [FIXME: exact ref missing]               |
| eMMC:                      | `Phison PS8211-0`                                                                                                                                                                                                         |
| 2.4GHz RF:                 | `Celeno CL2432` 3x3 802.11ac 2.4GHz RF chip ([celeno.com product page](https://www.celeno.com/products/cl2432))                                                                                                           |
| 5GHz RF:                   | `Celeno CL2440` 4x4 802.11ac Wave 2 5GHz RF chip ([celeno.com product page](https://www.celeno.com/products/cl2440))                                                                                                      |
| cable gateway SoC:         | `MaxLinear MXL277` cable gateway, front-end SoC designed for DOCSIS 3.1 ([maxlinear.com product page](https://www.maxlinear.com/product/access/cable-broadband/cable-front-ends/fsc-and-narrowband-tuners-demods/mxl277)) |
| cable upstream amplifier:  | `MaxLinear MXL236` PGA IC designed for DOCSIS 3.1 ([maxlinear.com product page](https://www.maxlinear.com/product/access/cable-broadband/cable-front-ends/upstream-amplifiers/mxl236))                                    |

## Firmware/Software

For documentation on the software see: [Software.md](./Software.md)

## Related and interesting stuff

- [blog.danman.eu reversing an 'Compal CH7465LG-LC'](https://blog.danman.eu/about-adding-a-static-route-to-my-docsis-modem/)
- ['Arris TG2492 Teardown' by Gertrude at mobile-computer-repairs.co.uk](https://www.mobile-computer-repairs.co.uk/blog/topic/29/routers/Arris-TG2492)
- [haxorware.com forum thread 'Arris TG2492'](http://www.haxorware.com/forums/showthread.php?tid=6860)
- [Database for identifing logos on IC's at famdom.com](<https://how-to.fandom.com/wiki/How_to_identify_integrated_circuit_(chip)_manufacturers_by_their_logos>)
- [Vodafone Kabel Deutschland pNTP Interface Specification v1.0.4](https://www.vodafone.de/media/downloads/pdf/VKD-DOCSIS-Interface-Specification-v1.04.pdf)
