# Hardware identification

![PCB front panel](img/pcb_front.png)

## Overview

1. CPU
2. RAM
3. Flash
4. 2.4 GHz RF chip
5. 5 GHz RF chip
6. ???Single Chip Power Management IC??? (only res found: [deviwiki.com search results](https://deviwiki.com/w/index.php?search=BD2650MWV)) [FIXME: place some better refs and infos]
7. Cable upstream amplifier
8. Cable gateway SoC
9. ???maybe the Ethernet chipset/driver/controller??? [FIXME: identify the chip and place some refs]
10. Subscriber Line IC
11. eMMC

![PCB front panel (marked)](img/pcb_front_marked.png)
![PCB back panel (marked)](img/pcb_back_marked.png)

## Identified Components

### CPU

`Intel FHCE2752M` (Intel Puma 7 SoC CE2752M) 2 cores, 2.5 GHz, Intel Atom Arch ([Intel Puma 7 product family page](https://ark.intel.com/content/www/de/de/ark/products/140087/intel-puma-7-family.html))

<details>
  <summary>Photo</summary>

![CPU](img/pcb_front_cpu.png)

</details>

### RAM

4x `Samsung K4B2G1646F-BYK0` ???Capacity used (4x512 MByte?)??? DDR3-RAM ([Samsung product page](https://www.samsung.com/semiconductor/dram/ddr3/K4B2G1646F-BYK0/))  [FIXME: exact capacity]

<details>
  <summary>Photo</summary>

![single RAM IC](img/pcb_front_ram_single.png)
![all RAM ICs](img/pcb_front_ram_multi.png)

</details>

### Flash

`Kioxia TC58NVG2S0HBAI4` 512 MByte SLC NAND EEPROM (Toshiba/[Kioxia product page](https://business.kioxia.com/en-us/memory/detail.TC58NVG2S0HBAI4.html))

<details>
  <summary>Photo</summary>

![Flash EEPROM](img/pcb_front_flash.png)

</details>

### 2.4 GHz RF chip

`Celeno CL2432` 3x3 802.11ac 2.4GHz RF chip ([celeno.com product page](https://www.celeno.com/products/cl2432))

<details>
  <summary>Photo</summary>

![2.4GHz chip](img/pcb_front_24GHz-rf.png)

</details>

### 5 GHz RF chip

`Celeno CL2440` 4x4 802.11ac Wave 2 5GHz RF chip ([celeno.com product page](https://www.celeno.com/products/cl2440))

<details>
  <summary>Photo</summary>

![5GHz chip](img/pcb_front_5GHz-rf.png)

</details>

### Power Management IC

`ROHM BD2650MV` [FIXME: infos needed]

<details>
  <summary>Photo</summary>

![Power management IC](img/pcb_front_power-mgt.png)

</details>

### Cable upstream amplifier

`MaxLinear MXL236` PGA IC designed for DOCSIS 3.1 ([maxlinear.com product page](https://www.maxlinear.com/product/access/cable-broadband/cable-front-ends/upstream-amplifiers/mxl236))

<details>
  <summary>Photo</summary>

![Cable upstream amplifier](img/pcb_front_cable-amplifier.png)

</details>

### Cable gateway SoC

`MaxLinear MXL277` cable gateway, front-end SoC designed for DOCSIS 3.1 ([maxlinear.com product page](https://www.maxlinear.com/product/access/cable-broadband/cable-front-ends/fsc-and-narrowband-tuners-demods/mxl277))

<details>
  <summary>Photo</summary>

![Cable gateway SoC](img/pcb_front_cable-gateway.png)

</details>

### Ethernetcontroller

[FIXME: infos and refs needed]

<details>
  <summary>Photo</summary>

![Ethernet Controller](img/pcb_front_ethernet-controller.png)

</details>

### Subscriber Line IC

`Microsemi ZL88107` Microsemi Corporation, ???maybe part of ZL880 series -> [product page](https://www.microchip.com/design-centers/interface-and-connectivity/line-circuits)??? [FIXME: exact ref and infos missing]

<details>
  <summary>Photo</summary>

![Subscriber Line IC](img/pcb_front_slic.png)

</details>

### eMMC

`Phison PS8211-0` [FIXME: exact infos and refs needed]

<details>
  <summary>Photo</summary>

![eMMC IC](img/pcb_back_eMMC.png)

</details>
