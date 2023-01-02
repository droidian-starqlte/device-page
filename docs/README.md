## Features & Usability

|                               	|    	|                                  	|    	|                      	|   	|
|-------------------------------	|----	|----------------------------------	|----	|----------------------	|---	|
| Manual brightnes              	|  ✅ 	| Battery lifetime > 24h from 100% 	|  ✅ 	| Automatic brightness  |  ✅ 	|
| No reboot needed for 1 week      	|  ❔	| Fingerprint reader  	                |  ✖️✖️   | Waydroid		|  ✅	|
| Torchlight                    	|  ✅	| Boot into UI                     	|  ✅ 	| GPS                 	|  ✅ 	|
| Vibration                     	|  ✅ 	| Hardware video playback          	|  ✅ 	| Proximity          	|  ✅ 	|
| Flashlight                    	|  ✅	| Anbox patches                    	|  ✅ 	| Rotation            	|  ✅ 	|
| Photo                         	|  ✅	| AppArmor patches                 	|  ✅ 	| Touchscreen          	|  ✅ 	|
| Video                         	|  ✅	| Battery percentage               	|  ✅ 	| Earphones           	|  ✅	|
| Switching between cameras     	|  ✅	| Offline charging                 	|  ✅	| Loudspeaker          	|  ✅	|
| Dual SIM functionality        	| ✖️ ✖️  	| Online charging                  	|  ✅ 	| Microphone          	|  ✅	|
| Carrier info, signal strength 	|  ✅ 	| SD card detection and access     	|  ✅ 	| Volume control       	|  ✅ 	|
| Data connection               	|  ✅ 	| RTC time                         	|  ✅ 	| Pin unlock           	|  ✅ 	|
| Incoming, outgoing calls      	|  ✅ 	| Shutdown / Reboot                	|  ✅ 	| ADB access          	|  ✖️✖️  	|
| MMS in, out                   	|  ❔ 	| Wireless External monitor        	|  ✖️✖️	| MTP access           	|  ✖️✖️  	|
| SMS in, out                    	|  ✅ 	| Bluetooth                        	|  ✅ 	| WiFi			|  ✅	|
| Change audio routings          	|  ✅	| Flight mode                      	|  ✅ 	| Hotspot		|  ✅	|
| Voice in calls                	|  ✅ 	|

- **✅** *Confirmed working.*
- **✅✖️** *Working to some extent but with issues.*
- **✖️** *Not Working.*
- **❔** *Not tested.*
- **✖️✖️** *Global issue.*

## Requirements
- Android 10 firmware for your device:
  - Redmi Note 7: https://xiaomifirmwareupdater.com/miui/lavender/stable/V11.0.6.0.PFGMIXM/

## Files
- Download the latest rootfs:  [droidian-OFFICIAL-phosh-phone-rootfs-api28-arm64-nightly_XXXXXXXX.zip](https://github.com/droidian-images/droidian/releases/tag/nightly).
- Download the adaptation script: [adaptation-surya-script.zip](https://github.com/droidian-lavender/adaptation-droidian-lavender/releases/download/adaptation/adaptation-droidian-lavender.zip).

## Installation
- Flash your favorite recovery ( TWRP Recommended ).
- Format userdata as ext4 from inside the recovery or via fastboot: `fastboot format:ext4 userdata`.
- Now boot into recovery.
- Go into sideload mode and sideload adaptation-droidian-garden.zip: `adb sideload adaptation-droidian-lavender.zip`
- Go into sideload mode and sideload droidian-OFFICIAL-phosh-phone-rootfs-api29-arm64-nightly_XXXXXXXX.zip: `adb sideload droidian-OFFICIAL-phosh-phone-rootfs-api29-arm64-nightly_XXXXXXXX.zip`

- Now boot into your device.
- *The first boot will take a while.*

## Notes
- The default password is `1234`.
- If you see a black screen, don't worry it takes a long time to boot.
- **Droidian GSIs are experimental! Bugs and missing features are expected.**

## Bugs
- Mobile data needs an APN to be set up from Settings -> Mobile -> Acess Point Names.
- Mobile data might stop working after making or recieving phone calls. Toggle Mobile Data from the settins off/on.
- Dual SIM functionality is currently not implemented in Phosh so only one SIM works at the moment.

## Final notes
- I'm not responsible for bricked devices, dead SD cards, thermonuclear war, or you getting fired because the alarm app failed.
- Please do some research if you have any concerns about features included in the products you find here before flashing it!
- YOU are choosing to make these modifications, and if you point the finger at me for messing up your device, I will laugh at you.

# Support
- Droidian telegram group: [@DroidianLinux](https://t.me/DroidianLinux).
