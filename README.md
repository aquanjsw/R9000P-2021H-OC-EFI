# MacOS 26 OC EFI for Legion R9000P 2021H (5800H + 3060 Laptop)

> [!TIP]
> The [nred](https://github.com/aquanjsw/R9000P-2021H-OC-EFI/tree/nred) branch can be used as a fallback EFI for init setup/debug as it need no extra setup within OS but provide a relatively smoother experience **in hybrid mode**.

> [!WARNING]
>
> - Replace the SMBIOS using [GenSMBIOS](https://github.com/corpnewt/gensmbios)

## Verification

|     | Component            | Model               |
| --- | -------------------- | ------------------- |
| ✅  | NVIDIA Driver        | 2.6.4               |
| ✅  | OS                   | 26.7.1              |
| ✅  | internal BOE monitor | 2560x1600@165hz     |
| ✅  | external monitor     | 2560x1440@60hz@hdmi |
| ✅  | CPU                  | 5800H               |
| ✅  | dGPU                 | 3060 Laptop         |
| ❌  | iGPU                 | Vega 8              |
| ✅  | SSD                  | SN730               |
| ✅  | WIFI / Bluetooth     | AX210               |
| ✅  | Audio                | ALC287              |
| ✅  | Trackpad             | -             |

## Tips

**OS install**

- Using hybird mode during OS install
- Turn to dGPU only mode after finishing the manual install steps in [nullmoth/nvidia-macos-driver](https://github.com/nullmoth/nvidia-macos-driver)
- Following [usbtoolbox/tool](https://github.com/usbtoolbox/tool) 's guide to replace `UTBMap.kext` before OS install

## Refs

- [nvidia driver](https://github.com/nullmoth/nvidia-macos-driver)
- [wifi](https://github.com/laobamac/itlwm/)
- [bluetooth](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/issues/505#issuecomment-3370000263)
- [audio](https://github.com/laobamac/SimpleHDA)
