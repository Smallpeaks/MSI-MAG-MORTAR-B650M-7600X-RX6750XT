# MSI-MAG-MORTAR-B650M-7600X-RX6950XT-MacOS 15.4 Completeness

**OpenCore : 1.0.5**

**macOS ：15.4**

**SMBIOS : MacPro7,1**

### Specification

| **Component**    | **Model**                    |
| ---------------- | -----------------------------|
| CPU              | AMD Ryzen 5 7600X            |
| Motherboard      | MSI(MAG) B650M MORTAR WIFI   |
| RAM              | XPG 32GB(16GB×2)DDR5 6000Mhz |
| Audio Chipset    | ALC4080 Codec                |
| GPU              | AMD Radeon RX 6950 XT 16G    |
| Ethernet         | RTL8125B 2.5Gbps LAN         |
| WiFi & Bluetooth | intel AX210                  |
| OS Disk(nvme)    | NVME XPG Gen4 1TB            |

### Bios Setup

  Based on Load Optimize defaults

- TMP (Disable)
- Secure Boot (Disable)
- Resize BAR (Disable)
- 4G Decoding (Disable)
- Change to CSM mode

Solution 1: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-carry; MacOS 15 requires Wi-Fi to be used with the Heliport app

Solution 2: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-carry; MacOS 15 requires OCLP patching here using option 2

If you want to achieve the additional function of air carry, you need to buy a NVME M.2 SSD to connect to the Heiguo wireless network card

By default, the boot can support independent graphics AMD Radeon RX 6950 XT 16G

### Works

- Audio
- RX 6950XT
- Ethernet
- USB  
- Wi-Fi
- Bluetooth
- Sleep wake-up is normal
- The GPU supports HDMI/DP display output
- I won't talk about them one by one

### OpenCore Configuration

### ACPI

| ACPIs                                    |
|------------------------------------------|
|  DSDT-MSI-MAG-B650M-BIOS-MORTAR          |
|  SSDT-AMD-Radeon-RX6650XT                |
|  SSDT-MSI-MAG-B650M-EC-MORTAR            |
|  SSDT-MSI-MAG-B650M-MORTAR               |

### Drivers

| Driver Name     |
|-----------------|
| HfsPlus         |
| OpenCanopy      |
| OpenRuntime     |
| ResetNvramEntry |
| ToggleSipEntry  |


### Changelog:
update Lilu.kext V1.7.1

update VirtualSMC.kext V1.3.7

update VoodooHDA.kext V2.9.9

update AppleMCEReporterDisabler.kext V1.2

update RestrictEvents.kext V1.1.6

update AMDRyzenCPUPowerManagement.kext V0.7.2

update SMCAMDProcessor.kext V0.3.3

update SMCRadeonGPU.kextV0.3.3

update NVMeFix.kext V1.1.3

update AMFIPass.kext V1.4.1

update FeatureUnlock.kext V1.1.8

update HibernationFixup.kext V1.5.4

update LucyRTL8125Ethernet.kext V1.2.2

update USBToolBox.kextV1.1.1

update UTBMap.kext V1.0

update AMDUSBX.kext V1.3.0b2

update IOSkywalkFamily.kext V1.0

update IO80211FamilyLegacy.kext V1200.12.2b1

update AirportItlwm15.4Sequoia.kext V2.4.0

update IntelBTPatcher.kext V2.5.0

update IntelBluetoothFirmware.kext V2.5.0

update BlueToolFixup.kext V2.6.9

update RadeonBoost.kext V1.0


若有其他问题请加Q群： 738882434
