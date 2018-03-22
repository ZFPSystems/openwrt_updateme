# OpenWRT updateme
Very simple script to update intalled packages on OpenWRT OS without hassle.

Author: Paolo Fabio Zaino
License: GPL v2

This script will detect all installed packages on your OpenWRT installation and will attempt to update them with the latest version (if any) in OPKG repository for your device.

NOTE: Before using this script make sure you have correctly configured and installed OpenWRT on your device and that opkg can reach the correct repository!

Please help me to improve this script with your suggestions and changes, thanks!
--------------------------------------------------------------------------------

## Installation
1) Clone this project on your computer and then upload the updateme script in your root directory on your OpenWRT device via scp.

2) Make sure the script has execution privileges by running:

   chmod +x ./updateme

3) You are ready to go!

## Usage
Just run the script as root by typing:

./updateme

