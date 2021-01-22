# Software identification

Latest firmware in Germany according to web interface is _AR01.02.068.11_092320_711.SIP.10 (01.02.068.11.EURO.SIP)_ as of 01/17/2021.

The following table lists details on the firmware versions and links to additional resources, like for example the source code and manual.

| Firmware              | Source                                                                                      | Manual |
| :-------------------- | :------------------------------------------------------------------------------------------ | ------ |
| 01.02.068.11.EURO.SIP | N/A                                                                                         | N/A    |
| 01.02.025             | https://sourceforge.net/projects/tg3442de.arris/files/TG3442DE_AR.01.02.025.tar.gz/download | N/A    |

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

## Used OSS components (01.02.068.11.EURO.SIP)

The information on used open source components lists following components

| Module                                | Version               |
| :------------------------------------ | :-------------------- |
| acpid                                 | 2.0.23                |
| ajaxfileupload.js                     |                       |
| apply_system_defaults                 |                       |
| arris-atom-kmod                       |                       |
| arris-kmod                            |                       |
| arris.js                              |                       |
| atom-swdl-utility                     |                       |
| attr                                  | 2.4.47                |
| avahi                                 | 0.6.31                |
| avro                                  | 1.8.1                 |
| base_95x.js                           |                       |
| base.js                               |                       |
| base64                                |                       |
| BaseUefiTianoCustomDecompressLib      |                       |
| bash                                  | 3.2.48                |
| Bind                                  | 9.9.5                 |
| bridge-utils                          | 1.5                   |
| busybox                               | 1.22                  |
| busybox                               | 1.22.1                |
| bzip2                                 | 1.0.6                 |
| c_registration                        |                       |
| c_rehash                              |                       |
| cable-netdev-mod                      | 0.0.3                 |
| cable-netdev-mod                      |                       |
| ccsp-common-library                   |                       |
| ccsp-cr                               |                       |
| ccsp-dmcli                            |                       |
| ccsp-gwprovapp                        |                       |
| ccsp-home-security                    |                       |
| ccsp-hotspot                          |                       |
| ccsp-hotspot-kmod                     |                       |
| ccsp-lm-lite                          |                       |
| ccsp-misc                             |                       |
| ccsp-moca                             |                       |
| ccsp-mta-agent                        |                       |
| ccsp-p-and-m                          |                       |
| ccsp-psm                              |                       |
| ccsp-safenat-broadband                |                       |
| ccsp-snmp-pa                          |                       |
| ccsp-tr069-pa                         |                       |
| ccsp-wecb-controller                  |                       |
| ccsp-wifi-agent                       |                       |
| CcspPhpExtension                      |                       |
| chosen.min.css                        |                       |
| ChvTbltDevicePkg                      |                       |
| cjson                                 | 1.0.0                 |
| cm                                    |                       |
| CMAgentSsp                            |                       |
| common                                |                       |
| Compatibility                         |                       |
| conntrack-tools                       | 1.4.0                 |
| cppp-linux-kernel                     |                       |
| CpuIoDxe                              |                       |
| cthelper                              | 1.0.0                 |
| cttimeout                             | 1.0.0                 |
| curl                                  | 7.35.0                |
| DatahubStatusCodeHandlerDxe           |                       |
| datapath                              |                       |
| datapipe-mod                          | 1.0.0.1               |
| dbridge_dlm                           |                       |
| dbus                                  | 1.6.18                |
| dhcpproxy                             |                       |
| dhcpv4c                               |                       |
| dibbler                               | 1.0.0RC2              |
| directconnect-dp                      |                       |
| dnsmasq                               | 2.78                  |
| docsis_fltr_class                     |                       |
| docsis_mac                            | mac_mngt_msg.h        |
| docsis_pp                             |                       |
| dropbear                              | 2017.75               |
| dspmod                                |                       |
| DxeImageVerificationLib               |                       |
| DxeTpm2MeasureBootLib                 |                       |
| e2fsprogs                             | 1.42.9                |
| ebtables                              | 2.0.10-4              |
| eglibc                                | 2.19                  |
| elessar.css                           |                       |
| elessar.min.js                        |                       |
| Engine_Pro_C_Src                      |                       |
| erouter_ni                            |                       |
| ethsw                                 |                       |
| excanvas.min.js                       |                       |
| execute_dir                           |                       |
| expat                                 | 2.1.0                 |
| ez-ipupdate                           | 3.0.11b7              |
| ezsp-host                             |                       |
| fcgi                                  | 2.4.0                 |
| firewall                              |                       |
| firewall_log                          |                       |
| flex                                  | 2.5.38                |
| gawk                                  | 3.1.5                 |
| gcc                                   | 4.8.2                 |
| gcc-runtime                           |                       |
| gim-proxy                             | gw_prov_abstraction.h |
| glib                                  | 2.38.2                |
| glib-networking                       | 2.38.0                |
| gnutls                                | 2.12.24               |
| gpio                                  |                       |
| gptfdisk                              | 1.0.0                 |
| gptfdisk                              | 1.0.1                 |
| gw_api_proxy                          | platform_hal.h        |
| gw_gim_proxy                          |                       |
| hal_isr                               |                       |
| hal_memory_map.h                      |                       |
| hal_mng_q                             |                       |
| hal_platform.h                        |                       |
| hal_soc_interface_driver              |                       |
| hal_types_api.h                       |                       |
| hal_types_ofdm.h                      |                       |
| hdparm                                | 9.43                  |
| heirloom-mailx                        | 12.5                  |
| hildrv-mod                            |                       |
| hostapd                               |                       |
| icctl                                 | kmalloc.h             |
| igd                                   |                       |
| iniparse                              |                       |
| iniparser                             |                       |
| intel_dns_app                         |                       |
| intelce-icc                           | kmalloc.c             |
| intelce-icc                           | kmalloc.h             |
| ipcplugin                             |                       |
| iperf                                 | 2.0.5                 |
| iperf                                 |                       |
| iperf3                                | 3.2                   |
| iproute2                              | 3.12.0                |
| ipsec-tools                           | 0.8.1                 |
| ipset                                 | 6.29                  |
| iptables                              | 1.4.21                |
| iqvlinux                              |                       |
| jansson                               | 2.7                   |
| jqplot.canvasAxisLabelRenderer.min.js |                       |
| jqplot.canvasTextRenderer.min.js      |                       |
| jqplot.cursor.min.js                  |                       |
| jquery-1.4.2.min.js                   | 1.4.2                 |
| jquery-1.7.2.min.js                   | 1.7.2                 |
| jquery-ui-1.8.21.custom.css           | 1.8.21                |
| jquery-ui-1.8.21.custom.min.js        | 1.8.21                |
| jquery-ui-1.8.4.custom.css            | 1.8.4                 |
| jquery-ui-1.8.5.custom.min.js         | 1.8.5                 |
| jquery.alerts.progress.js             |                       |
| jquery.chosen.js                      |                       |
| jquery.ciscoExt.js                    |                       |
| jquery.foldertree.js                  |                       |
| jquery.highContrastDetect.js          |                       |
| jquery.jqplot.min.css                 |                       |
| jquery.jqplot.min.js                  |                       |
| jquery.md5.js                         |                       |
| jquery.radioswitch.js                 |                       |
| jquery.ui.accordion.css               |                       |
| jquery.ui.all.css                     |                       |
| jquery.ui.autocomplete.css            |                       |
| jquery.ui.base.css                    |                       |
| jquery.ui.button.css                  |                       |
| jquery.ui.core.css                    |                       |
| jquery.ui.datepicker.css              |                       |
| jquery.ui.dialog.css                  |                       |
| jquery.ui.progressbar.css             |                       |
| jquery.ui.resizable.css               |                       |
| jquery.ui.selectable.css              |                       |
| jquery.ui.slider.css                  |                       |
| jquery.ui.tabs.css                    |                       |
| jquery.ui.theme.css                   |                       |
| jquery.validate.js                    |                       |
| jquery.virtualDialog.js               |                       |
| json-c                                | 0.11                  |
| json2.js                              |                       |
| jstree.js                             |                       |
| kmod                                  |                       |
| kernel-driver                         |                       |
| kmod                                  | tools                 |
| libAhncCosaApi                        |                       |
| libcap                                | 2.22                  |
| libdaemon                             | 0.14                  |
| libevent                              | 2.0.21-stable         |
| libffi                                | 3.0.13                |
| libgcrypt                             | 1.5.3                 |
| libgpg-error                          | 1.12                  |
| libicc                                | kmalloc.c             |
| libicc                                | kmalloc.h             |
| libipcplugin-api                      |                       |
| libkmod                               |                       |
| libmnl                                | 1.0.3                 |
| libnetfilter_conntrack                | 1.0.2                 |
| libnetfilter-cthelper                 |                       |
| libnetfilter-cttimeout                |                       |
| libnetfilter-queue                    |                       |
| libnfnetlink                          | 1.0.1                 |
| libnfsidmap                           | 0.25                  |
| libnl                                 | 3.2.22                |
| libpcap                               | 1.5.3                 |
| libproxy                              | 0.4.11                |
| libtasn1                              | 4.8                   |
| libtirpc                              | 0.2.4                 |
| libudhcp4plugin                       |                       |
| libupnp                               | 1.6.18                |
| libusb                                | 1.0.9                 |
| libwatchdog                           |                       |
| libxml2                               | 2.9.1                 |
| lighttpd                              | 1.4.33                |
| linux                                 | 3.12.14               |
| linux                                 | 3.12.59               |
| Linux                                 | Headers               |
| Linux-PAM                             | 1.1.6                 |
| log4c                                 | 1.2.3                 |
| logrotate                             | 3.8.7                 |
| lsof                                  | 4.87                  |
| LzmaCustomDecompressLib               |                       |
| lzo                                   | 2.06                  |
| macclone                              |                       |
| mcs-mod                               |                       |
| MdeModulePkg                          |                       |
| MdePkg                                |                       |
| mesh-agent                            |                       |
| miniupnpd                             | 1.8.20141022          |
| mldproxy                              |                       |
| mldproxy                              | config.c              |
| mldproxy                              | confread.c            |
| mldproxy                              | inet6_opt.c           |
| mldproxy                              | logger.c              |
| moca                                  |                       |
| moca_ni                               |                       |
| moca-netdev                           | 1.0.0.0               |
| mso_mgmt                              |                       |
| mta                                   |                       |
| mtani                                 |                       |
| mxp                                   |                       |
| ncsdk                                 | rijndael-alg-fst.c    |
| ncsdk                                 | rijndael-alg-fst.h    |
| ncsdk                                 | rijndael-api-fst.c    |
| ncsdk                                 | rijndael-api-fst.h    |
| ncurses                               | 5.9                   |
| neon                                  | 0.30.0                |
| net-snmp                              | 5.7.2                 |
| netip-sec-server                      |                       |
| netkit-tftp                           | 0.17                  |
| netutils_util                         |                       |
| newhost                               |                       |
| nfs-utils                             | 1.2.9                 |
| nss-mdns                              | 0.10                  |
| ntp                                   | 4.2.6p5               |
| openssl                               | 0.9.8ze               |
| openssl                               | 1.0.2h                |
| packagegroup-core-boot                |                       |
| pciutils                              | 3.2.1                 |
| pcre                                  | 8.34                  |
| pdsp                                  |                       |
| pdspdrv-mod                           |                       |
| perl                                  | 5.14.3                |
| php                                   | 5.4.14                |
| PhysicalPresencePei                   |                       |
| platform                              |                       |
| PlatformSetupDxe                      |                       |
| pmon                                  |                       |
| popt                                  | 1.16                  |
| portmap                               | 6.0                   |
| powertop                              | 2.5                   |
| pp                                    |                       |
| ppdrv-mod                             |                       |
| puma-litepath                         |                       |
| puma-power-app                        |                       |
| puma-power-app                        | acpi_ids.c            |
| puma-power-app                        | acpi_ids.h            |
| puma-power-app                        | libnetlink.c          |
| puma-power-app                        | libnetlink.h          |
| quagga                                | 0.99.21               |
| rdk-logger                            |                       |
| rdkb-cable-modem-hal                  | cm_hal.h              |
| rdkb-dhcp-hal                         | dhcpv4c_api.h         |
| rdkb-moca-hal                         | moca_hal.h            |
| rdkb-mta-hal                          | mta_hal.h             |
| rdkb-platform-hal                     | platform_hal.h        |
| rdkb-vlan-hal                         | vlan_hal.h            |
| rpcbind                               | 0.2.1                 |
| ruli                                  | 0.36                  |
| sec-linux-kernel-p7                   |                       |
| service_ipv6                          |                       |
| service_multinet                      |                       |
| service_routed                        |                       |
| service_wan                           |                       |
| services                              |                       |
| sgc                                   |                       |
| shadow                                | 4.1.4.3               |
| shadow-securetty                      | 4.1.4.3               |
| ShellPkg                              |                       |
| sjcl.js                               |                       |
| skis                                  | lipr                  |
| snmp                                  |                       |
| spawn-fcgi                            | 1.6.3                 |
| sqlite                                | autoconf-3120200      |
| squashfs                              | 4.2                   |
| ssmpt                                 | 2.64                  |
| strace                                | 4.8                   |
| style.css                             |                       |
| swapi-mod                             |                       |
| swctl                                 |                       |
| synopsys-gbe                          | 4.10a-1               |
| synopsysgbe-mod                       | 4.10a-1               |
| sys_resource                          |                       |
| syscfg                                |                       |
| sysevent                              |                       |
| sysfsutils                            | 2.1.0                 |
| sysklogd                              | 1.5                   |
| systemd                               | 216                   |
| tcp_wrappers                          | 7.6                   |
| Tcpdump                               | 4.3.0                 |
| telehal                               |                       |
| test-and-diagnostic                   |                       |
| ti_kerberos                           | ossl.c                |
| ti_kerberos                           | ossl.h                |
| ti-dhcpv6                             |                       |
| tinyxml                               | 2.6.2                 |
| toe                                   |                       |
| TR-181                                |                       |
| trigger                               |                       |
| udhcp                                 |                       |
| UefiCpuPkg                            |                       |
| ulog                                  |                       |
| underscore.js                         |                       |
| us_pdsp_driver                        |                       |
| usbutils                              | 7                     |
| utapi                                 |                       |
| utctx                                 |                       |
| util-linux                            | 2.24.1                |
| utilityFunctions.js                   |                       |
| utils                                 |                       |
| vlan                                  |                       |
| voiceni                               |                       |
| watchdogd                             |                       |
| webgui                                | cmn                   |
| wifi_hal                              | celeno                |
| wifi-proxy                            |                       |
| wireless_tools                        | 30.pre9               |
| xdns                                  |                       |
| xml                                   |                       |
| XZ                                    | Utils                 |
| yajl                                  | 1.0.9                 |
| ZigBeeDeviceEmberZcl                  |                       |
| zlib                                  | 1.2.8                 |
