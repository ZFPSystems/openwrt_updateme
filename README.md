# OpenWRT updateme
Very simple script to update intalled packages on OpenWRT OS without hassle.

Author: Paolo Fabio Zaino
License: GPL v3

This script will detect all installed packages on your OpenWRT installation and will attempt to update them with the latest version (if any) in OPKG repository for your device.

NOTE: Before using this script make sure you have correctly configured and installed OpenWRT on your device and that opkg can reach the correct repository!

Please help me to improve this script with your suggestions and changes, thanks!
--------------------------------------------------------------------------------

## Installation
1) Clone this project on your computer and then upload the updateme script in your root directory on your OpenWRT device via scp.

2) Make sure the script has execution privileges by running:
   ```
   chmod u+x ./updateme
   ```
3) You are ready to go!

## Usage
Just run the script as root by typing:

```
./updateme
```

Output can be quite long:
```
...
[Starting checking for upgrades]
Please wait this could take a while...
Upgrading dnsmasq on root from 2.78-1 to 2.78-6...
Downloading http://downloads.lede-project.org/releases/17.01.4/packages/arm_cortex-a9_vfpv3/base/dnsmasq_2.78-6_arm_cortex-a9_vfpv3.ipk
Configuring dnsmasq.
Collected errors:
 * resolve_conffiles: Existing conffile /etc/config/dhcp is different from the conffile in the new package. The new conffile will be placed at /etc/config/dhcp-opkg.
Upgrading dropbear on root from 2017.75-2 to 2017.75-4...
Downloading http://downloads.lede-project.org/releases/17.01.4/packages/arm_cortex-a9_vfpv3/base/dropbear_2017.75-4_arm_cortex-a9_vfpv3.ipk
Configuring dropbear.
Collected errors:
 * resolve_conffiles: Existing conffile /etc/dropbear/dropbear_rsa_host_key is different from the conffile in the new package. The new conffile will be placed at /etc/dropbear/dropbear_rsa_host_key-opkg.
 * resolve_conffiles: Existing conffile /etc/config/dropbear is different from the conffile in the new package. The new conffile will be placed at /etc/config/dropbear-opkg.
Upgrading hostapd-common on root from 2016-12-19-ad02e79d-6 to 2016-12-19-ad02e79d-7...
Downloading http://downloads.lede-project.org/releases/17.01.4/packages/arm_cortex-a9_vfpv3/base/hostapd-common_2016-12-19-ad02e79d-7_arm_cortex-a9_vfpv3.ipk
Configuring hostapd-common.
...
```

## Tested on
This script is tested and works fine on OpenWRT and LEDE. For more info about which versions you may want to have a look at the releases. Generally I test it on a bunch of old routers and some new router, if and when I have time.

