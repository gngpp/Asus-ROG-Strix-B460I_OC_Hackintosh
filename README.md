[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.1-yellowgreen)](https://github.com/zf1976/ROG-Strix-B460I_OC_Hackintosh/releases/tag/0.6.5)
[![macOS](https://img.shields.io/badge/macOS-12.4-orange)](https://www.apple.com/macos/catalina/)
[![MODEL](https://img.shields.io/badge/Model-B460I-blue)](https://www.asus.com/Motherboards/ROG-STRIX-B460-I-GAMING/)

<img src="images/neofetch.png">

##  i5 10400 + ASUS ROG STRIX B460-I GAMING 核显 独显Radeon RX 560 4 GB Hackintosh EFI
> 支持OTA升级，建议使用镜像升级。
- Catalina 10.15.x
- BugSur 11.x
- Monterey 12.4

---


### 电脑配置

| 规格     | 详细信息                                     |
| -------- | ---------------------------------------- |
| 主板型号 | Asus ROG Strix B460-I             |
| 处理器   | Intel Core i5 10400           |
| 内存     | Asgard 32GB 2x16GB DDR4 2666Mhz                 |
| 电源     | 益衡7145b 1U                    |
| 机箱     | Formula 2S                    |
| 显卡     | Radeon RX 560 4 GB ITX && HD630                    |
| 硬盘     | WDS500G3X0C-00SJG0 512GB M.2 NVMe                  |
| 声卡     | Realtek ALCS1220A (Layout 7)                    |
| 网卡&蓝牙     | DW1560 + NGFF M.2 Adapter                             |
| 板载网卡 | Intel® i219-V 1Gb Ethernet |
| 显示器   | Q2490W1  |

---

### BIOS设置

**关闭：**
- Fast Boot
- VT-d
- CSM
- Intel SGX

**开启：**
- VT-x
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: other system
- DVMT Pre-Allocated (iGPU Memory): 64MB

---

### 完美程度
- 核显硬解加速正常，显存1536MB
- 睡眠正常
- _CPU_ 睿频正常，单核4.3，全核4.0
- 传感器正常工作、_CPU_ 温度、_SSD_ 温度风扇转速均可获取（通过iStat Menus查看）
- 定制USB映射正常
  USB3.2Gen2x2未测试，没有这么高的设备，不过是系统识别出单独走线，符合官方描述，应该可达到20Gbps）
- 有线网正常工作
- 驱动 _DW1560 WIFI_ ，蓝牙正常

---

### FAQ
- 记得修改platforminfo里面的串号，以免不能登陆app store
- 显示器输出支持HDMI DP 核显独显都支持
- 若有bug并且可以修复，记得提PR
- 如果使用核显，独显缓冲帧建议删除。
- 替换EFI后在终端记得执行:`sudo kextcache -i/`
---
