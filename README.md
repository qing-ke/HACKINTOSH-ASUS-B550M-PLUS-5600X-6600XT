# hackintosh  ASUS-b550m-plus-5600x-6600xt

## 硬件配置
- 主板：华硕 ASUS TUF B550M-WIFI
- CPU：AMD 5600X
- 显卡：MSI6600XT魔龙
- 内存：英睿达 铂胜 DDR4 3200 16GB * 2
- 硬盘：浦科特M7VC 256G SATA3固态硬盘
- 网卡：BCM94360CD
- 引导：OpenCore 0.8.2
- 系统版本：macOS Monterey 12.2.1 

## BIOS设置（设置前先恢复默认）
#### disable 禁用
- Fast Boot
- CSM
- SerialPort
#### enable 开启
- Above 4G decoding
- AMD SVM
- EHCI/XHCI Hand-off
#### 其他
- SecureBoot: other types
- SATA：AHCI

## 第一次遇到的问题，仅记录
1. 为了装mac买的网卡，装上之后WIN下WI-FI不识别。
	 解决：在主板里将PCIE16_2设置成x2
2. 装完mac后，蓝牙不识别。
   解决方案：之前使用的<<完美USB>>两个USB2.0扩展不可用，替换成当前的解决了
3. 使用OC引导进入WIN黑屏
   解决方案：未解决，当前去掉WIN引导，配置Scan Policy 3080963，等待时间0，不显示引导界面。
   