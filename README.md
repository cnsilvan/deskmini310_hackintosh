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

## Works

* [x] Ethernet/WIFI/Bluetooth/Audio/USB/Sensors

* [x] DP/HDMI dual monitor output

* [x] Shutdown、Sleep

## Notes

* After macOS installed done ([Tutorial](https://www.tonymacx86.com/)), please open `config.plist` and  fill few SMBIOS info by Clover Configurator.

* If you use `BCM94352Z` , please move BCM94352Z/* to CLOVER/kexts/Other.

* If you need to move CLOVER/kexts/Other/* to /L/E&/S/L/E, please modify `InjectKexts` to `Detect` in `config.plist` by Clover Configurator.

## Tips

* If you use `Chrome` , it is recommended to turn off `Chrome` completely when using `IGPU` operations(PS/FCP etc).

* I will write some detailed tutorials (How to install macos and configure clover, etc.) in my free time, and this repository will be continuously updated until I  use the Deskmini310 no longer.

## ChangeLog

| Date      | Content                                                              |
|-----------|----------------------------------------------------------------------|
| 2019.7.28 | update clover  5018 & upgrade Mojave 10.14.6 , everything is alright |

