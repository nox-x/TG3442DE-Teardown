# Software identification

Latest firmware in Germany according to web interface is `AR01.02.068.11_092320_711.SIP.10` as of 01/17/2021.

The following table lists details on the firmware versions and links to additional resources, like for example the source code and manual.

| Firmware                 | Source                                                                                      | Manual | Branding      | Firmware (long)                       |
| :----------------------- | :------------------------------------------------------------------------------------------ | ------ | :------------ | :------------------------------------ |
| `01.01.117.01.EURO`      | N/A                                                                                         | N/A    | Vodafone (DE) | `AR01.01.117.01_091718_70.PC20.10`    |
| `01.02.025`              | https://sourceforge.net/projects/tg3442de.arris/files/TG3442DE_AR.01.02.025.tar.gz/download | N/A    | Arris         | N/A                                   |
| `01.02.037.08.EURO.PC20` | N/A                                                                                         | N/A    | Vodafone (DE) | `AR01.02.037.08_121719_711.PC20.10`   |
| `01.02.068.11.EURO.SIP`  | N/A                                                                                         | N/A    | N/A           | `AR01.02.068.11_092320_711.SIP.10`    |

# Software

Software is maintained by the cable service provider and will be pushed to the devices over DOCSIS management options. The source code for the firmware is released to Sourceforge and can be downloaded [here](https://sourceforge.net/arris/tg3442de/home/Home/).

## Installation of source code

This section explains how you can grab the source code and compile it to a working firmware image.

### Prerequirements for installation

- Firmware source code
- [Yocto/BitBake build system](https://www.yoctoproject.org/docs/1.6/mega-manual/mega-manual.html)

### Download of source code

The easiest way to download the software is via wget or curl

`wget https://sourceforge.net/projects/tg3442de.arris/files/latest/download`

or

`curl -L https://sourceforge.net/projects/tg3442de.arris/files/latest/download > source.tar.gz`

After the download, decompress the source code via tar command.

`tar xvfz source.tar.gz`

The source will be decompressed to a subfolder.

# Webinterface

The router runs a lighthttpd service with a web gui. After login the webinterface features following main options

- Overview (http://192.168.0.1/?overview)
- Phone (http://192.168.0.1/?phone_call_log)
- Internet (http://192.168.0.1/?net_firewall)
- WLAN (http://192.168.0.1/?wifi_general)
- Settings (http://192.168.0.1/?settings_device)
- Status & Help (http://192.168.0.1/?status_status)

## Used OSS components

The information on used open source components lists following components for the specific firmware versions

| Module                                | `01.01.117.01.EURO`             | `01.02.037.08.EURO.PC20`        | `01.02.068.11.EURO.SIP` |
| :------------------------------------ | :------------------------------ | :------------------------------ | :---------------------- |
| acpid                                 | 2.0.23                          | 2.0.23                          | 2.0.23                  |
| ajaxfileupload.js                     |                                 |                                 |                         |
| apply_system_defaults                 |                                 |                                 |                         |
| arris-atom-kmod                       |                                 |                                 |                         |
| arris-kmod                            | 1.0                             | 1.0                             |                         |
| arris-syscfg                          | 1.0                             | 1.0                             |                         |
| arris-webgui                          | 1.0                             | 1.0                             |                         |
| arris.js                              |                                 |                                 |                         |
| atom-swdl-utility                     |                                 |                                 |                         |
| attr                                  |                                 |                                 | 2.4.47                  |
| avahi-daemon                          | 0.6.31                          | 0.6.31                          | 0.6.31                  |
| avro-c                                | 1.8.1                           | 1.8.1                           | 1.8.1                   |
| base-files                            | 3.0.14                          | 3.0.14                          |                         |
| base-passwd                           | 3.5.29                          | 3.5.29                          |                         |
| base_95x.js                           |                                 |                                 |                         |
| base.js                               |                                 |                                 |                         |
| base64                                |                                 |                                 |                         |
| BaseUefiTianoCustomDecompressLib      |                                 |                                 |                         |
| bash                                  | 3.2.48                          | 3.2.48                          | 3.2.48                  |
| Bind                                  |                                 |                                 | 9.9.5                   |
| bridge-utils                          | 1.5                             | 1.5                             | 1.5                     |
| busybox                               | 1.22.1                          | 1.22.1                          | 1.22.1                  |
| busybox-syslog                        | 1.22.1                          | 1.22.1                          |                         |
| busybox-udhcpc                        | 1.22.1                          | 1.22.1                          |                         |
| bzip2                                 |                                 |                                 | 1.0.6                   |
| c_registration                        |                                 |                                 |                         |
| c_rehash                              |                                 |                                 |                         |
| ca-certificates                       | 20130610                        | 20130610                        |                         |
| cable-netdev-mod                      | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              | 0.0.3                   |
| ccsp-cm-agent                         | rdkb-2.1-20161219+gitbadcb81b14 | rdkb-2.1-20161219+gitbadcb81b14 |                         |
| ccsp-common-library                   |                                 |                                 |                         |
| ccsp-common-startup                   | rdkb-2.1-20161219+git7ca2f51897 | rdkb-2.1-20161219+git7ca2f51897 |                         |
| ccsp-cr                               | rdkb-2.1-20161219+git8cf7808be7 | rdkb-2.1-20161219+git8cf7808be7 |                         |
| ccsp-dmcli                            | rdkb-2.1-20161219+git4e33c62f49 | rdkb-2.1-20161219+git4e33c62f49 |                         |
| ccsp-gwprovapp                        | rdkb-2.1-20161219+git96e1d74ecc | rdkb-2.1-20161219+git96e1d74ecc |                         |
| ccsp-home-security                    | rdkb-2.1-20161219+git83f0a38d9b | rdkb-2.1-20161219+git83f0a38d9b |                         |
| ccsp-hotspot                          | rdkb-2.1-20161219+gitf138e1ea6c | rdkb-2.1-20161219+gitf138e1ea6c |                         |
| ccsp-hotspot-kmod                     | rdkb-2.1-20161219+gitf138e1ea6c | rdkb-2.1-20161219+gitf138e1ea6c |                         |
| ccsp-lm-lite                          | rdkb-2.1-20161219+gitecdc780ca9 | rdkb-2.1-20161219+gitecdc780ca9 |                         |
| ccsp-misc                             | rdkb-2.1-20161219+git96a383207d | rdkb-2.1-20161219+git96a383207d |                         |
| ccsp-moca                             |                                 |                                 |                         |
| ccsp-mta-agent                        | rdkb-2.1-20161219+gitc0d7114df7 | rdkb-2.1-20161219+gitc0d7114df7 |                         |
| ccsp-p-and-m                          | rdkb-2.1-20161219+gitd15535c6b9 | rdkb-2.1-20161219+gitd15535c6b9 |                         |
| ccsp-psm                              | rdkb-2.1-20161219+gitbc0d3fc507 | rdkb-2.1-20161219+gitbc0d3fc507 |                         |
| ccsp-safenat-broadband                |                                 |                                 |                         |
| ccsp-snmp-pa                          | rdkb-2.1-20161219+git3d91c13dbf | rdkb-2.1-20161219+git3d91c13dbf |                         |
| ccsp-tr069-pa                         | rdkb-2.1-20161219+gitd9443d4c1d | rdkb-2.1-20161219+gitd9443d4c1d |                         |
| ccsp-wecb-controller                  | rdkb-2.1-20161219+git92f1b70fd5 | rdkb-2.1-20161219+git92f1b70fd5 |                         |
| ccsp-wifi-agent                       | rdkb-2.1-20161219+gita18235c15e | rdkb-2.1-20161219+gita18235c15e |                         |
| CcspPhpExtension                      |                                 |                                 |                         |
| chosen.min.css                        |                                 |                                 |                         |
| ChvTbltDevicePkg                      |                                 |                                 |                         |
| cjson                                 |                                 |                                 | 1.0.0                   |
| cm                                    |                                 |                                 |                         |
| CMAgentSsp                            |                                 |                                 |                         |
| common                                |                                 |                                 |                         |
| Compatibility                         |                                 |                                 |                         |
| conntrack-tools                       | 1.4.0                           | 1.4.0                           | 1.4.0                   |
| cppp-linux-kernel                     | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| cppp-linux-user                       | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| CpuIoDxe                              |                                 |                                 |                         |
| cthelper                              |                                 |                                 | 1.0.0                   |
| cttimeout                             |                                 |                                 | 1.0.0                   |
| curl                                  | 7.35.0                          | 7.35.0                          | 7.35.0                  |
| DatahubStatusCodeHandlerDxe           |                                 |                                 |                         |
| datapath                              | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| datapipe-mod                          | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              | 1.0.0.1                 |
| dbridge_dlm                           |                                 |                                 |                         |
| dbus-1                                | 1.6.18                          | 1.6.18                          | 1.6.18                  |
| dhcpproxy                             |                                 |                                 |                         |
| dhcp-client                           | 4.3.0                           | 4.3.0                           |                         |
| dhcp-server                           | 4.3.0                           | 4.3.0                           |                         |
| dhcp-server-config                    | 4.3.0                           | 4.3.0                           |                         |
| dhcpv4c                               |                                 |                                 |                         |
| dibbler                               | 1.0.0RC2                        | 1.0.0RC2                        | 1.0.0RC2                |
| directconnect-dp                      | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| dnsmasq                               |                                 |                                 | 2.78                    |
| docsis_fltr_class                     |                                 |                                 |                         |
| docsis_mac                            |                                 |                                 | mac_mngt_msg.h          |
| docsis_pp                             |                                 |                                 |                         |
| dropbear                              | 2014.63                         | 2014.63                         | 2017.75                 |
| dspmod                                |                                 |                                 |                         |
| DxeImageVerificationLib               |                                 |                                 |                         |
| DxeTpm2MeasureBootLib                 |                                 |                                 |                         |
| e2fsprogs                             | 1.42.9                          | 1.42.9                          | 1.42.9                  |
| ebtables                              | 2.0.10-4                        | 2.0.10-4                        | 2.0.10-4                |
| eglibc                                |                                 |                                 | 2.19                    |
| elessar.css                           |                                 |                                 |                         |
| elessar.min.js                        |                                 |                                 |                         |
| Engine_Pro_C_Src                      |                                 |                                 |                         |
| erouter_ni                            |                                 |                                 |                         |
| ethsw                                 |                                 |                                 |                         |
| excanvas.min.js                       |                                 |                                 |                         |
| execute_dir                           |                                 |                                 |                         |
| expat                                 |                                 |                                 | 2.1.0                   |
| ez-ipupdate                           | 3.0.11b7                        | 3.0.11b7                        | 3.0.11b7                |
| ezsp-host                             |                                 |                                 |                         |
| fcgi                                  |                                 | 2.4.0                           | 2.4.0                   |
| firewall                              |                                 |                                 |                         |
| firewall_log                          |                                 |                                 |                         |
| flex                                  | 2.5.38                          | 2.5.38                          | 2.5.38                  |
| gawk                                  |                                 |                                 | 3.1.5                   |
| gcc                                   |                                 |                                 | 4.8.2                   |
| gcc-runtime                           |                                 |                                 |                         |
| gim-proxy                             |                                 |                                 | gw_prov_abstraction.h   |
| glib                                  |                                 |                                 | 2.38.2                  |
| glib-networking                       | 2.38.0                          | 2.38.0                          | 2.38.0                  |
| gnutls                                |                                 |                                 | 2.12.24                 |
| gpio                                  |                                 |                                 |                         |
| gptfdisk                              | 1.0.0                           | 1.0.0/1.0.1                     | 1.0.0                   |
| gw_api_proxy                          |                                 |                                 | platform_hal.h          |
| gw_gim_proxy                          |                                 |                                 |                         |
| hal                                   | rdkb-2.1-20161219+gitf72fc24d2e | rdkb-2.1-20161219+gitf72fc24d2e |                         |
| hal_isr                               |                                 |                                 |                         |
| hal_memory_map.h                      |                                 |                                 |                         |
| hal_mng_q                             |                                 |                                 |                         |
| hal_platform.h                        |                                 |                                 |                         |
| hal_soc_interface_driver              |                                 |                                 |                         |
| hal_types_api.h                       |                                 |                                 |                         |
| hal_types_ofdm.h                      |                                 |                                 |                         |
| hdparm                                | 9.43                            | 9.43                            | 9.43                    |
| heirloom-mailx                        |                                 | git+intelsdk-7.0ga              | 12.5                    |
| hildrv-mod                            | git+intelsdk-7.0ga              | 1.0+0                           |                         |
| hostapd                               |                                 |                                 |                         |
| icctl                                 |                                 |                                 | kmalloc.h               |
| igd                                   |                                 |                                 |                         |
| iksemel                               | 1.5                             | 1.5                             |                         |
| iniparser                             |                                 |                                 |                         |
| initscripts                           | 1.0                             | 1.0                             |                         |
| initscripts-functions                 | 1.0                             | 1.0                             |                         |
| intel-dns-app                         | 1.0+intelsdk0                   | 1.0+intelsdk0                   |                         |
| intelce-icc                           |                                 |                                 | kmalloc.c/h             |
| ipcplugin                             |                                 |                                 |                         |
| iperf                                 | 2.0.5                           | 2.0.5                           | 2.0.5                   |
| iperf3                                |                                 |                                 | 3.2                     |
| iproute2                              | 3.12.0                          | 3.12.0                          | 3.12.0                  |
| ipsec-tools                                                            || 0.8.1                           | 0.8.1                   |
| ipset                                 | 6.29                            | 6.29                            | 6.29                    |
| iptables                              | 1.4.21                          | 1.4.21                          | 1.4.21                  |
| iqvlinux-linux-kernel                 | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| jansson                               |                                 |                                 | 2.7                     |
| jqplot.canvasAxisLabelRenderer.min.js |                                 |                                 |                         |
| jqplot.canvasTextRenderer.min.js      |                                 |                                 |                         |
| jqplot.cursor.min.js                  |                                 |                                 |                         |
| jquery-1.4.2.min.js                   |                                 |                                 | 1.4.2                   |
| jquery-1.7.2.min.js                   |                                 |                                 | 1.7.2                   |
| jquery-ui-1.8.21.custom.css           |                                 |                                 | 1.8.21                  |
| jquery-ui-1.8.21.custom.min.js        |                                 |                                 | 1.8.21                  |
| jquery-ui-1.8.4.custom.css            |                                 |                                 | 1.8.4                   |
| jquery-ui-1.8.5.custom.min.js         |                                 |                                 | 1.8.5                   |
| jquery.alerts.progress.js             |                                 |                                 |                         |
| jquery.chosen.js                      |                                 |                                 |                         |
| jquery.ciscoExt.js                    |                                 |                                 |                         |
| jquery.foldertree.js                  |                                 |                                 |                         |
| jquery.highContrastDetect.js          |                                 |                                 |                         |
| jquery.jqplot.min.css                 |                                 |                                 |                         |
| jquery.jqplot.min.js                  |                                 |                                 |                         |
| jquery.md5.js                         |                                 |                                 |                         |
| jquery.radioswitch.js                 |                                 |                                 |                         |
| jquery.ui.accordion.css               |                                 |                                 |                         |
| jquery.ui.all.css                     |                                 |                                 |                         |
| jquery.ui.autocomplete.css            |                                 |                                 |                         |
| jquery.ui.base.css                    |                                 |                                 |                         |
| jquery.ui.button.css                  |                                 |                                 |                         |
| jquery.ui.core.css                    |                                 |                                 |                         |
| jquery.ui.datepicker.css              |                                 |                                 |                         |
| jquery.ui.dialog.css                  |                                 |                                 |                         |
| jquery.ui.progressbar.css             |                                 |                                 |                         |
| jquery.ui.resizable.css               |                                 |                                 |                         |
| jquery.ui.selectable.css              |                                 |                                 |                         |
| jquery.ui.slider.css                  |                                 |                                 |                         |
| jquery.ui.tabs.css                    |                                 |                                 |                         |
| jquery.ui.theme.css                   |                                 |                                 |                         |
| jquery.validate.js                    |                                 |                                 |                         |
| jquery.virtualDialog.js               |                                 |                                 |                         |
| json-c                                | 0.11                            | 0.11                            | 0.11                    |
| json2.js                              |                                 |                                 |                         |
| jstree.js                             |                                 |                                 |                         |
| kmod                                  |                                 |                                 |                         |
| kernel-driver                         |                                 |                                 |                         |
| kernel-module-ak8975                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-ansi-cprng              | 3.12.14                         | 3.12.14                         |                         |
| kernel-module-arris                   | 1.0                             | 1.0                             |                         |
| kernel-module-avalanche-cnid          | 1.0+intelsdk0                   | 1.0+intelsdk0                   |                         |
| kernel-module-bd6107                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-bma180                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-brmtumod                | rdkb-2.1-20161219+gitf138e1ea6c | rdkb-2.1-20161219+gitf138e1ea6c |                         |
| kernel-module-c3p-test-driver         | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-cable-netdev            | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-configfs                | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-cordic                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-cppp                    | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-crc8                    | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-dpd-netdev              | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-dwc-eth-qos             | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-dwc-eth-qos-gbe         | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-eeprom-93cx6            | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-g-mass-storage          | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-generic-adc-batter y    | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-generic-bl              | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-gpio-backlight          | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-hid-elo                 | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-hid-huion               | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-hid-magicmouse          | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-hid-ntrig               | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-hid-xinmo               | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-hil-drv                 | git+intelsdk-7.0ga              | git+intelsdk-7.0ga / 1.0+0      |                         |
| kernel-module-ideapad-slidebar        | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-inv-mpu6050             | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-ip6table-raw            | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-iptable-raw             | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-iqvlinux                | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-isofs                   | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-isp1704-charger         | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-lcd                     | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-libcomposite            | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-lv5207lp                | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-mcp320x                 | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-mdio-bitbang            | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-moca-netdev-driver      | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-nau7802                 | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-nlmon                   | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-pch-dma                 | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-pdsp-drv                | git+intelsdk-7.0ga              | git+intelsdk-7.0ga / 1.0+0      |                         |
| kernel-module-platform-lcd            | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-pp-drv                  | git+intelsdk-7.0ga              | git+intelsdk-7.0ga / 1.0+0      |                         |
| kernel-module-puma-lpal               | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-puma7-pp-init           | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-romfs                   | 3.12.14                         | 3.12.14                         |                         |
| kernel-module-sec-kernel              | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-sgc-drv                 | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-sr9700                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-tmp006                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-toe-drv                 | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-udf                     | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-ushc                    | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-veth                    | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-vub300                  | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-wbsd                    | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-module-wifi-mux                | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-wifi-proxy-netdev       | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| kernel-module-xt-ct                   | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kernel-modules                        | 3.12.59+gitAUTOINC+0fd090c8b6   | 3.12.59+gitAUTOINC+0fd090c8b6   |                         |
| kmod                                  | 16+gitAUTOINC+36c4bb928a        | 16+gitAUTOINC+36c4bb928a        |                         |
| libAhncCosaApi                        |                                 |                                 |                         |
| libattr1                              | 2.4.47                          | 2.4.47                          |                         |
| libavahi-common3                      | 0.6.31                          | 0.6.31                          |                         |
| libavahi-core7                        | 0.6.31                          | 0.6.31                          |                         |
| libavcodec53                          | 0.8.9                           | 0.8.9                           |                         |
| libavformat53                         | 0.8.9                           | 0.8.9                           |                         |
| libavutil51                           | 0.8.9                           | 0.8.9                           |                         |
| libblkid1                             | 2.24.1                          | 2.24.1                          |                         |
| libbz2-0                              | 1.0.6                           | 1.0.6                           |                         |
| libc-extra-nss                        | 2.19                            | 2.19                            |                         |
| libc6                                 | 2.19                            | 2.19                            |                         |
| libc6-dev                             | 2.19                            | 2.19                            |                         |
| libcap2                               | 2.22                            | 2.22                            | 2.22                    |
| libccsp-common0                       | rdkb-2.1-20161219+git7ca2f51897 | rdkb-2.1-20161219+git7ca2f51897 |                         |
| libcidn1                              | 2.19                            | 2.19                            |                         |
| libcom-err2                           | 1.42.9                          | 1.42.9                          |                         |
| libcrypto1.0.0                        | 1.0.2h                          | 1.0.2h                          |                         |
| libcunit-dev                          | 2.1-3                           | 2.1-3                           |                         |
| libcunit1                             | 2.1-3                           | 2.1-3                           |                         |
| libcurl4                              | 7.35.0                          | 7.35.0                          |                         |
| libdaemon0                            | 0.14                            | 0.14                            | 0.14                    |
| libdbus-1-3                           | 1.6.18                          | 1.6.18                          |                         |
| libe2p2                               | 1.42.9                          | 1.42.9                          |                         |
| libevent                              | 2.0.21                          | 2.0.21                          | 2.0.21-stable           |
| libexif12                             | 0.6.21                          | 0.6.21                          |                         |
| libexpat1                             | 2.1.0                           | 2.1.0                           |                         |
| libext2fs2                            | 1.42.9                          | 1.42.9                          |                         |
| libffi6                               | 3.0.13                          | 3.0.13                          | 3.0.13                  |
| libflac8                              | 1.3.0                           | 1.3.0                           |                         |
| libgcrypt11                           | 1.5.3                           | 1.5.3                           | 1.5.3                   |
| libglib-2.0-0                         | 2.38.2                          | 2.38.2                          |                         |
| libgnutls26                           | 2.12.23                         | 2.12.23                         |                         |
| libgpg-error0                         | 1.12                            | 1.12                            | 1.12                    |
| libgssdp-1.0-3                        | 0.14.10                         | 0.14.10                         |                         |
| libicc                                |                                 |                                 |                         |
| libid3tag0                            | 0.15.1b                         | 0.15.1b                         |                         |
| libipcplugin-api                      |                                 |                                 |                         |
| libjansson4                           | 2.4                             | 2.4                             |                         |
| libjpeg8                              | 8d+1.3.1                        | 8d+1.3.1                        |                         |
| libkmod                               | 16+gitAUTOINC+36c4bb928a        | 16+gitAUTOINC+36c4bb928a        |                         |
| liblzma                               | 5.1.3alpha                      | 5.1.3alpha                      |                         |
| liblzo                                | 2.06                            | 2.06                            |                         |
| libmnl                                | 1.0.3                           | 1.0.3                           | 1.0.3                   |
| libmount                              | 2.24.1                          | 2.24.1                          |                         |
| libmtp-common                         | 1.1.5                           | 1.1.5                           |                         |
| libmtp-runtime                        | 1.1.5                           | 1.1.5                           |                         |
| libmtp9                               | 1.1.5                           | 1.1.5                           |                         |
| libncurses5                           | 5.9                             | 5.9                             |                         |
| libncursesw5                          | 5.9                             | 5.9                             |                         |
| libneon27                             | 0.30.0                          | 0.30.0                          |                         |
| libnetfilter-conntrack                | 1.0.2                           | 1.0.2                           | 1.0.2                   |
| libnetfilter-cthelper                 | 1.0.0                           | 1.0.0                           |                         |
| libnetfilter-cttimeout                | 1.0.0                           | 1.0.0                           |                         |
| libnetfilter-queue                    | 1.0.2                           | 1.0.2                           |                         |
| libnetsnmp30                          | 5.7.2                           | 5.7.2                           |                         |
| libnfnetlink                          | 1.0.1                           | 1.0.1                           | 1.0.1                   |
| libnfsidmap                           | 0.25                            | 0.25                            | 0.25                    |
| libnl                                 | 3.2.22                          | 3.2.22                          | 3.2.22                  |
| libnss-mdns                           | 0.10                            | 0.10                            |                         |
| libogg0                               | 1.3.1                           | 1.3.1                           |                         |
| libpam                                | 1.1.6                           | 1.1.6                           |                         |
| libpam-runtime                        | 1.1.6                           | 1.1.6                           |                         |
| libpcap                               | 1.5.3                           | 1.5.3                           | 1.5.3                   |
| libpci3                               | 3.2.1                           | 3.2.1                           |                         |
| libpcre                               | 8.34                            | 8.34                            |                         |
| libpcreposix0                         | 8.34                            | 8.34                            |                         |
| libperl5                              | 5.14.3                          | 5.14.3                          |                         |
| libpopt0                              | 1.16                            | 1.16                            |                         |
| libproxy                              | 0.4.11                          | 0.4.11                          | 0.4.11                  |
| libsoup-2.4                           | 2.48.1                          | 2.48.1                          |                         |
| libsqlite3-0                          | 3.12.2                          | 3.12.2                          |                         |
| libssl1.0.0                           | 1.0.2h                          | 1.0.2h                          |                         |
| libsysfs2                             | 2.1.0                           | 2.1.0                           |                         |
| libsystemd0                           | 216+gitAUTOINC+5d0ae62c66       | 216+gitAUTOINC+5d0ae62c66       |                         |
| libtasn1                              | 3.4                             | 3.4                             | 4.8                     |
| libtheora                             | 1.1.1                           | 1.1.1                           |                         |
| libthread-db1                         | 2.19                            | 2.19                            |                         |
| libtinfo5                             | 5.9                             | 5.9                             |                         |
| libtinyxml2.6.2                       | 2.6.2                           | 2.6.2                           |                         |
| libtirpc                              | 0.2.4                           | 0.2.4                           | 0.2.4                   |
| libudhcp4plugin                       |                                 |                                 |                         |
| libupnp                               | 1.6.18                          | 1.6.18                          | 1.6.18                  |
| libusb                                | 1.0.9                           | 1.0.9                           | 1.0.9                   |
| libuuid1                              | 2.24.1                          | 2.24.1                          |                         |
| libvorbis                             | 1.3.4                           | 1.3.4                           |                         |
| libwatchdog                           |                                 |                                 |                         |
| libwrap0                              | 7.6                             | 7.6                             |                         |
| libx264-133                           | r2265+gitAUTOINC+ffc3ad4945     | r2265+gitAUTOINC+ffc3ad4945     |                         |
| libxml2                               | 2.9.1                           | 2.9.1                           | 2.9.1                   |
| libz                                  | 1.2.8                           | 1.2.8                           |                         |
| lighttpd                              | 1.4.33                          | 1.4.33                          | 1.4.33                  |
| lighttpd-module-access                | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-accesslog             | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-auth                  | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-cgi                   | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-csrf                  | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-dirlisting            | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-fastcgi               | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-indexfile             | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-redirect              | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-rewrite               | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-secdownload           | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-setenv                | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-ssi                   | 1.4.33                          | 1.4.33                          |                         |
| lighttpd-module-staticfile            | 1.4.33                          | 1.4.33                          |                         |
| linux                                 | 3.12.14                         | 3.12.14                         | 3.12.14                 |
| linux                                 |                                 | kernel-3.12.59-yocto-standard   | 3.12.59                 |
| Linux                                 |                                 |                                 |                         |
| Linux-PAM                             |                                 |                                 | 1.1.6                   |
| linux-libc-headers-dev                | 3.12.59                         | 3.12.59                         |                         |
| load-datapipe                         | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| load-modules                          | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| log4c                                 | 1.2.3                           | 1.2.3                           | 1.2.3                   |
| logrotate                             | 3.8.7                           | 3.8.7                           | 3.8.7                   |
| lrzsz                                 | 0.12.20                         | 0.12.20                         |                         |
| lsof                                  | 4.87                            | 4.87                            | 4.87                    |
| LzmaCustomDecompressLib               |                                 |                                 |                         |
| lzo                                   |                                 |                                 | 2.06                    |
| m4                                    | 1.4.9                           | 1.4.9                           |                         |
| macclone                              |                                 |                                 |                         |
| mailx                                 | 12.5                            | 12.5                            |                         |
| mcs-mod                               |                                 |                                 |                         |
| MdeModulePkg                          |                                 |                                 |                         |
| MdePkg                                |                                 |                                 |                         |
| mesh-agent                            |                                 |                                 |                         |
| minidlna                              | 1.1.5                           | 1.1.5                           |                         |
| miniupnpd                             | 1.8                             | 1.8                             | 1.8.20141022            |
| mldproxy                              | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| moca                                  |                                 |                                 |                         |
| moca_ni                               |                                 |                                 |                         |
| moca-netdev                           |                                 |                                 | 1.0.0.0                 |
| moca-netdev-mod                       | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| mso_mgmt                              |                                 |                                 |                         |
| mta                                   |                                 |                                 |                         |
| mtani                                 |                                 |                                 |                         |
| mtd-utils-ubifs                       | 1.5.0+gitAUTOINC+dcea43eba9     | 1.5.0+gitAUTOINC+dcea43eba9     |                         |
| mtp-tools                             | 1.1.5                           | 1.1.5                           |                         |
| mxp                                   |                                 |                                 |                         |
| ncsdk                                 |                                 | rijndael-alg-fst.c/h, rijndael-api-fst.c/h |
| ncurses                               | 5.9                             | 5.9                             | 5.9                     |
| neon                                  |                                 |                                 | 0.30.0                  |
| net-snmp                              | 5.7.2                           | 5.7.2                           | 5.7.2                   |
| netbase                               | 5.2                             | 5.2                             |                         |
| netip-sec-server                      | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| netkit-tftp                           | 0.17                            | 0.17                            | 0.17                    |
| netutils_util                         |                                 |                                 |                         |
| network                               | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| newhost                               |                                 |                                 |                         |
| nfs-utils                             | 1.2.9                           | 1.2.9                           | 1.2.9                   |
| nss-mdns                              |                                 |                                 | 0.10                    |
| ntp                                   | 4.2.6p5                         | 4.2.6p5                         | 4.2.6p5                 |
| ntp-tickadj                           | 4.2.6p5                         | 4.2.6p5                         |                         |
| nvram                                 | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| openssl                               |                                 |                                 | 0.9.8ze                 |
| openssl                               | 1.0.2h                          | 1.0.2h                          | 1.0.2h                  |
| openssl-conf                          | 1.0.2h                          | 1.0.2h                          |                         |
| os-release                            | 1.0                             | 1.0                             |                         |
| packagegroup-base                     | 1.0                             | 1.0                             |                         |
| packagegroup-base-ext2                | 1.0                             | 1.0                             |                         |
| packagegroup-base-extended            | 1.0                             | 1.0                             |                         |
| packagegroup-base-ipv6                | 1.0                             | 1.0                             |                         |
| packagegroup-base-nfs                 | 1.0                             | 1.0                             |                         |
| packagegroup-base-usbhost             | 1.0                             | 1.0                             |                         |
| packagegroup-core-boot                | 1.0                             | 1.0                             |                         |
| packagegroup-distro-base              | 1.0                             | 1.0                             |                         |
| packagegroup-machine-base             | 1.0                             | 1.0                             |                         |
| pam-plugin-deny                       | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-env                        | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-faildelay                  | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-group                      | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-lastlog                    | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-limits                     | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-listfile                   | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-mail                       | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-motd                       | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-nologin                    | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-permit                     | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-rootok                     | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-securetty                  | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-shells                     | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-unix                       | 1.1.6                           | 1.1.6                           |                         |
| pam-plugin-warn                       | 1.1.6                           | 1.1.6                           |                         |
| pciutils                              | 3.2.1                           | 3.2.1                           | 3.2.1                   |
| pciutils-ids                          | 3.2.1                           | 3.2.1                           |                         |
| pcregrep                              | 8.34                            | 8.34                            | 8.34                    |
| pdsp                                  |                                 |                                 |                         |
| pdspdrv-mod                           | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| perl                                  | 5.14.3                          | 5.14.3                          | 5.14.3                  |
| php                                   |                                 |                                 | 5.4.14                  |
| php-cgi                               | 5.4.14                          | 5.4.14                          |                         |
| PhysicalPresencePei                   |                                 |                                 |                         |
| platform                              |                                 |                                 |                         |
| PlatformSetupDxe                      |                                 |                                 |                         |
| pmon                                  |                                 |                                 |                         |
| popt                                  |                                 |                                 | 1.16                    |
| portmap                               | 6.0                             | 6.0                             | 6.0                     |
| powertop                              | 2.5                             | 2.5                             | 2.5                     |
| pp                                    |                                 |                                 |                         |
| ppdrv-mod                             | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| puma-litepath                         | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| puma-power-app                        | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| quagga                                | 0.99.21                         | 0.99.21                         | 0.99.21                 |
| quagga-ripd                           | 0.99.21                         | 0.99.21                         |                         |
| quagga-ripngd                         | 0.99.21                         | 0.99.21                         |                         |
| rdk-logger                            |                                 |                                 |                         |
| rdkb-cable-modem-hal                  |                                 |                                 | cm_hal.h                |
| rdkb-dhcp-hal                         |                                 |                                 | dhcpv4c_api.h           |
| rdkb-moca-hal                         |                                 |                                 | moca_hal.h              |
| rdkb-mta-hal                          |                                 |                                 | mta_hal.h               |
| rdkb-platform-hal                     |                                 |                                 | platform_hal.h          |
| rdkb-vlan-hal                         |                                 |                                 | vlan_hal.h              |
| rpcbind                               | 0.2.1                           | 0.2.1                           | 0.2.1                   |
| ruli                                  |                                 |                                 | 0.36                    |
| run-postinsts                         | 1.0                             | 1.0                             |                         |
| sched                                 | 1.0                             | 1.0                             |                         |
| sec-linux-kernel-p7                   | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| service_ipv6                          |                                 |                                 |                         |
| service_multinet                      |                                 |                                 |                         |
| service_routed                        |                                 |                                 |                         |
| service_wan                           |                                 |                                 |                         |
| services                              |                                 |                                 |                         |
| sgc                                   |                                 |                                 |                         |
| sgc-mod                               | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| shadow                                | 4.1.4.3                         | 4.1.4.3                         | 4.1.4.3                 |
| shadow-securetty                      | 4.1.4.3                         | 4.1.4.3                         | 4.1.4.3                 |
| ShellPkg                              |                                 |                                 |                         |
| sjcl                                  | 1.0.6+gitAUTOINC+51ae8f8c92     | 1.0.6+gitAUTOINC+51ae8f8c92     |                         |
| skis                                  |                                 |                                 | lipr                    |
| smartmontools                         | 6.2                             | 6.2                             |                         |
| snmp                                  |                                 |                                 |                         |
| spawn-fcgi                            | 1.6.3                           | 1.6.3                           | 1.6.3                   |
| sqlite                                |                                 |                                 | autoconf-3120200        |
| squashfs                              | 4.2                             | 4.2                             | 4.2                     |
| ssmpt                                 | 2.64                            | 2.64                            | 2.64                    |
| strace                                | 4.8                             | 4.8                             | 4.8                     |
| style.css                             |                                 |                                 |                         |
| swapi-mod                             |                                 |                                 |                         |
| swctl                                 |                                 |                                 |                         |
| synopsys-gbe                          |                                 |                                 | 4.10a-1                 |
| synopsysgbe-mod                       | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              | 4.10a-1                 |
| sys-resource                          | rdkb-2.1-20161219+git4e9cded35f | rdkb-2.1-20161219+git4e9cded35f |                         |
| syscfg                                |                                 |                                 |                         |
| sysevent                              |                                 |                                 |                         |
| sysfsutils                            | 2.1.0                           | 2.1.0                           | 2.1.0                   |
| sysklogd                              | 1.5                             | 1.5                             | 1.5                     |
| sysstat                               | 10.2.1                          | 10.2.1                          |                         |
| systemd                               | 216+gitAUTOINC+5d0ae62c66       | 216+gitAUTOINC+5d0ae62c66       | 216                     |
| systemd-binfmt                        | 216+gitAUTOINC+5d0ae62c66       | 216+gitAUTOINC+5d0ae62c66       |                         |
| systemd-compat-units                  | 1.0                             | 1.0                             |                         |
| systemd-serialgetty                   | 1.0                             | 1.0                             |                         |
| tcp_wrappers                          |                                 |                                 | 7.6                     |
| tcpdump                               | 4.3.0                           | 4.3.0                           | 4.3.0                   |
| telehal                               |                                 |                                 |                         |
| test-and-diagnostic                   | rdkb-2.1-20161219+gitdfbeb26dd1 | rdkb-2.1-20161219+gitdfbeb26dd1 |                         |
| ti_kerberos                           |                                 |                                 | ossl.c                  |
| ti_kerberos                           |                                 |                                 | ossl.h                  |
| ti-dhcpv6                             | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| ti-udhcp                              | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| tinyxml                               |                                 |                                 | 2.6.2                   |
| toe                                   |                                 |                                 |                         |
| toe-mod                               | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| TR-181                                |                                 |                                 |                         |
| trigger                               |                                 |                                 |                         |
| udhcp                                 |                                 |                                 |                         |
| udev                                  | 216+gitAUTOINC+5d0ae62c66       | 216+gitAUTOINC+5d0ae62c66       |                         |
| UefiCpuPkg                            |                                 |                                 |                         |
| ulog                                  |                                 |                                 |                         |
| underscore.js                         |                                 |                                 |                         |
| update-alternatives-opkg              | 0.1.8+gitAUTOINC+c33b217016     | 0.1.8+gitAUTOINC+c33b217016     |                         |
| us_pdsp_driver                        |                                 |                                 |                         |
| usbutils                              | 7                               | 7                               | 7                       |
| usbutils-ids                          | 7                               | 7                               |                         |
| utapi                                 |                                 |                                 |                         |
| utctx                                 |                                 |                                 |                         |
| util-linux                            |                                 |                                 | 2.24.1                  |
| util-linux-agetty                     | 2.24.1                          | 2.24.1                          |                         |
| util-linux-losetup                    | 2.24.1                          | 2.24.1                          |                         |
| util-linux-swaponoff                  | 2.24.1                          | 2.24.1                          |                         |
| util-linux-umount                     | 2.24.1                          | 2.24.1                          |                         |
| utilityFunctions.js                   |                                 |                                 |                         |
| utils                                 |                                 |                                 |                         |
| utopia                                | rdkb-2.1-20161219+git961c1d4294 | rdkb-2.1-20161219+git961c1d4294 |                         |
| version-puma7-Router                  | 1.0                             | 1.0                             |                         |
| vlan                                  |                                 |                                 |                         |
| voiceni                               |                                 |                                 |                         |
| volatile-binds                        | 1.0                             | 1.0                             |                         |
| vsftpd                                | 3.0.0                           | 3.0.0                           |                         |
| watchdogd                             | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| webgui                                |                                 |                                 | cmn                     |
| wifi_hal                              |                                 |                                 | celeno                  |
| wifi-proxy                            | git+intelsdk-7.0ga              | git+intelsdk-7.0ga              |                         |
| wireless-tools                        | 30.pre9                         | 30.pre9                         | 30.pre9                 |
| xdns                                  |                                 |                                 |                         |
| xml                                   |                                 |                                 |                         |
| XZ                                    |                                 |                                 | Utils                   |
| yajl                                  | 1.0.9                           | 1.0.9                           | 1.0.9                   |
| ZigBeeDeviceEmberZcl                  |                                 |                                 |                         |
| zlib                                  |                                 |                                 | 1.2.8                   |
