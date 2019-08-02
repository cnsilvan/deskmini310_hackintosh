# Hackintosh your Deskmini310

## Configuration

| Specifications | Detail                                                                                    |
|----------------|-------------------------------------------------------------------------------------------|
| CPU            | INTEL I7-8700                                                                             |
| RAM            | ADATA DDR4 2666MHz 16GB × 2                                                               |
| SSD            | WD SN750 512GB M.2 PCIE                                                                   |
| WIFI/BT        | BCM94360CS2                                                                               |
| Cooler         | ID-COOLING IS40x                                                                          |
| EX-USB2.0      | [taobao](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.5d642e8dpFbnJC&id=546924712980) |

The EFI support 9th/8th cpu and other RAM/SSD , see [asrock](https://www.asrock.com/nettop/Intel/DeskMini%20310%20Series/index.asp#Support)

## BIOS

version：P3.4（support P4.x）

* Advanced
  * Chipset Configuration
    * Onboard HD Audio: Enabled
  * USB Configuration
    * XHCI Hand-off: Enabled
  * Super IO Configuration
    * Serial Port: Disabled  
* Security
  * Secure Boot: Disabled(by default)

Other Configurations by default

## Works

* [x] Ethernet/WIFI/Bluetooth/Audio/USB/Sensors

* [x] DP/HDMI dual monitor output

* [x] Shutdown、Sleep

## Notes

* After macOS installed done ([Installation Guide](https://www.tonymacx86.com/threads/unibeast-install-macos-mojave-on-any-supported-intel-based-pc.259381/)), please open `config.plist` and  fill few SMBIOS info by Clover Configurator.

* If you use `BCM94352Z` , please move BCM94352Z/* to CLOVER/kexts/Other.

* If you need to move CLOVER/kexts/Other/* to /L/E&/S/L/E, please modify `InjectKexts` to `Detect` in `config.plist` by Clover Configurator.

## Tips

* If you use `Chrome` , it is recommended to turn off `Chrome` completely when using `IGPU` operations(PS/FCP etc).

* I will write some detailed tutorials (How to install macos and configure clover, etc.) in my free time, and this repository will be continuously updated until I  use the Deskmini310 no longer.

## Issues

Occasionally restart, but I think this is an inevitable problem for Hackintosh , Fortunately, it happens very rarely.

## Why Hackintosh

Because We Can！

## ChangeLog

| Date      | Content                                                              |
|-----------|----------------------------------------------------------------------|
| 2019.7.28 | update clover  5018 & upgrade Mojave 10.14.6（Supplemental update has not been tested） , everything is alright |
| 2019.7.31 | update clover  5033                                                  |
