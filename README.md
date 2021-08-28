## 这里是Dell vostro 3578 黑果的efi（可下载文件的仓库）

需要预览EFI内的文件 请移步至此仓库https://github.com/ABCDFAS/vostro-3578-hackintosh-efi/

（此clover年久失修 因转opencore 此引导暂停维护 但仍可安装Catalina Mojave）

接下来是之前的我的描述

这个efi 适用于dell vostro 3578 

本机配置：

| CPU  | i5-8250u                                        |
| ---- | ----------------------------------------------- |
| 内存 | 4GB DDR4 2400                                   |
| 硬盘 | 256GB 镁光SATA SSD                              |
| 显卡 | 核显 UHD620<br />独显Radeon 520（黑果无法驱动） |
| 声卡 | ALC236 layout-id: `16`                          |

- 功能列表
  - 核显驱动成功 显示2048mb
  - 声卡已经完美 使用applealc.kext 耳机切换正常
  - 网卡以太网可以的 无线我上了94360cs2 正常
  - 亮度已修复 可大幅度调
  - usb驱动已成功
  - 蓝牙正常
  - 触控板支持Apple多点式触控
  - 电池显示正常
  - 睡眠基本正常
  - 注意：如果触控板不能用请用终端输入命令来重建缓存 sudo kextcache -i/

不工作：独显

bios设置 csm关闭 uefi打开 secure boot关闭

clover版本 5103

2020/03/13更新：kext简化 解决可能因为触控板而导致的卡屏死机问题 将EFI内容打包成ZIP形式 有效解决部分下载不完整问题

2020/03/31更新：更新clover版本为5107 whatevergreen.kext为1.3.7 解决10.15.4卡+++
