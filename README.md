# Dell Inspiron 5482 2-in-1 Hackintosh (BigSur)

**CPU**: Intel Core i7-8565U  
**GPU**: Intel UHD Graphics 620  
**RAM**: 12 GB 2400 MHz DDR4   
**Wifi/BT Card**: Intel ...    

**SMBIOS**: MacbookPro15,2

✔️ Wifi/Bluetooth  
✔️ Wake/Sleep  
✔️ All USB Ports functional  
✔️ SD-Card Reader (USB Mapped)  
✔️ Camera  
✔️ Brightness control including shorcut keys  

⚠️ Battery life untested  
⚠️ HDMI Ouput untested  
⚠️ Recovery is not included in the repository

# Recovery
Complete your bootable USB by following this [official guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html#downloading-macos).

# BIOS Settings
__Secure Boot__: Disabled  
__SATA Operation__: AHCI  
__Intel SGX__: Disabled  
__VT for Direct I/O (VT-D)__: Enabled  

# Post-Install
### Sleep/Wake
[Source](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html)
```Shell
sudo pmset autopoweroff 0
sudo pmset powernap 0
sudo pmset standby 0
sudo pmset proximitywake 0
sudo pmset tcpkeepalive 0
```

### Audio (ALC236)
[Source](https://dortania.github.io/OpenCore-Post-Install/universal/audio.html#testing-your-layout)
```
layout 3, 11, 12, 13, 14, 15, 16, 18, 36, 54, 99
```

# Notes
- Trackpad settings are only available when battery is present.


