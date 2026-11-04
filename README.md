# Project Silicium UEFI for ARM64-Based Devices

> **HackiOS REDMI K90 移植分支：`k90-port`。** 本仓库是 [Project-Silicium/Mu-Silicium](https://github.com/Project-Silicium/Mu-Silicium) 的副本：`main` 是上游 `42fe563` 的导入，`k90-port` 增加 REDMI K90（annibale，SM8750）的 `annibalePkg`，以及在 BDS 里启动 XNU loader 的 BootManager 改动，用来构建 [HackiOS K90 移植](https://github.com/iola1999/hackios-redmi-k90-annibale)驻留 loader 镜像里的 UEFI。标签 `loader-v16` 是 loader v6～v16 镜像所用 FD 的源码状态。原许可证和版权声明保留。
>
> 高通 DXE 驱动来自子模块 `Binaries`（[Project-Silicium/Device-Binaries](https://github.com/Project-Silicium/Device-Binaries)）。annibalePkg 沿用同为 SM8750 的 OnePlus 13R（`dodge`）的驱动，构建前需要 `ln -s dodge Binaries/annibale`。构建步骤见顶层工作区的 [annibale UEFI 构建说明](https://github.com/iola1999/hackios-redmi-k90-annibale/blob/main/docs/analysis/annibale-uefi-build.md)。

<!-- ![Banner](https://github.com/Project-Silicium/Mu-Silicium/blob/main/Resources/Pictures/Banner.png) -->

## Description

This Project focuses on Making ARM-Based Devices Boot Operating Systems like Windows or Linux using Custom UEFI Firmware.

## Resources

- [Status](Status.md)
- [Building](Building.md)
- [Guides](https://github.com/Project-Silicium/Guides/blob/main/README.md)
- [Discord Server](https://discord.gg/Dx2QgMx7Sv)

## Frequently asked Questions

### **Is my Device Supported in this Project?**
- To Check if your Device is Supported, Take a Look at the Status Page Referenced in the Section Above.

### **What do I do if my Device isn't Supported in this Project?**
- We made some Guides that Explain How to Port your Device that are Referenced in the Section Above.

## Credits

[Microsoft](https://github.com/microsoft/) for their [Project Mu](https://microsoft.github.io/mu/) which Powers this Project. <br>
[WOA-Project](https://github.com/WOA-Project/) for their [mu_andromeda_platforms](https://github.com/WOA-Project/mu_andromeda_platforms/) which is used as Base for this Project. <br>
[Project Aloha](https://github.com/Project-Aloha/) for their [mu_aloha_platforms](https://github.com/Project-Aloha/mu_aloha_platforms/) which is used as Reference for some SoCs. <br>
[Open Surface RT](https://openrt.gitbook.io/open-surfacert/) for their Help on Tegra Related Stuff.

[sonic011gamer](https://github.com/sonic011gamer/) and [halal-beef](https://github.com/halal-beef/) for their Amazing Work on Exynos Related Stuff.

## License

All code except drivers in `GPLDrivers` & `GPLApplications` & `GPLLibrary` directories are licensed under BSD-2-Clause. <br />
GPL Drivers are licensed under `GPLv2` or later license.
