# Dell-5558-EFI
戴尔灵越15-5558黑苹果EFI，90%完美

电脑配置：加了4G内存，无线拆了原有的AC3160，17块包邮了平民网卡DW1707AR9565，双固态（Win10+Mac），拆掉光驱加了一块固态

| 配置项 | 配置说明 |
| :----: | :----: |
| 电脑型号 | 戴尔 Inspiron 5558 笔记本电脑  (扫描时间：2019年04月07日) |
| 操作系统 | 10.14.6(18G87) |
| 处理器 |       英特尔 Core i5-5200U @ 2.20GHz 双核|
| 主板 |        戴尔 0V7MX2 ( 英特尔 Broadwell-U - 5th Generation Intel Core Premium SKU - 9CC3 笔记本芯片组 )|
|内存|        8 GB ( 海力士 DDR3L 1600MHz )|
|主硬盘|        东芝 THNSNJ128GCSU ( 128 GB / 固态硬盘 )|
|显卡|        独显 Nvidia GeForce 920M ( 2 GB )  集显 HD5500|
|显示器 |      友达 AUO40EC ( 15.5 英寸  )|
|声卡  |      ALC255|
|网卡    |    无线 AR9565  有线 RTL8100|

安装镜像：黑果小兵10.14.6（18G87）请自行移步黑果小兵部落阁下载 clover已自行升级为5033

正常功能：

1、核显驱动正常，用的EFI里config.plist

2、USB2.0，3.0正常，facetime摄像正常

3、声卡使用APPLEALC，在ACPI里勾选修复HPET,声卡ID填3，勾选重置HDA，搭配APPLEALC可原生驱动声卡，需要在设置面板里把声音平衡拉到最左或最右声音才纯正

4、睡眠唤醒正常。亮度调节删除COLVER里有关亮度驱动，config里ACPI添加PNLF,有小太阳

5、HDMI可以输出，我用的HDMI转VGA，1366✖768低分屏看着难受，可外接1080P屏幕

6、有线无线正常，DW1707速度够用,clover里面有WiFi和蓝牙驱动，但是蓝牙用不了，可折腾下DW1820A，反正我没成功

存在问题：

1、HDMI外接屏颜色暗一层

2、开机第二段会有类似8苹果一闪而过，但又看不见完整的8个苹果，没有解决但不影响开机和正常使用

3、蓝牙无法找到硬件，在10.13.6和10.14..4一样情况

PS：

个人感觉90%完美，没事别乱升级clover。装机或者升级系统，务必在clover启动界面手动选择clover_for_update.plist，直到装完或升级完进入系统后，进入系统后,进入系统后,再次重启可使用config.plist驱动核显和声卡等。MAC的隔空接力什么的没试过，蓝牙用不了。目前已经可以满足日常使用，所以没有追求极致完美，无线网卡接口类型：ngff m2

这个仓库里没有DW1707的驱动，移步远景[DW1707网卡驱动](http://bbs.pcbeta.com/viewthread-1811188-1-1.html)

珍爱生命，不要熬夜折腾