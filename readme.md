# 华硕ASUS TUF B360M PLUS GMAING S
继承于[@qzz0518](https://github.com/qzz0518/hackintosh_9400f_b360_vega56)，但配件略有不同，所有独立一个仓库，便于自己维护。

## 具体配置如下：
| 硬件 | 型号 | 
| - | :-: |
| 主板 | 华硕ASUS TUF B360M PLUS GAMING S |
| 芯片 | INTEL i3 9100F |
| 显卡 | 铭影 RX560 4G |
| 内存 | 威刚+金士顿 DDR4 2400 8G*2 |
| 固态 | 台电 Teclast 240G NP800 |
| 机箱 | 乔思伯 w2 |
| 散热 | 酷冷T400 |

## 体验
nodejs web全栈开发。
本来有mini 18款i3钙版，自己加到32G内存。
但是每天背来背去有点嫌累，再买一台又过于奢侈，所以动了黑苹果的念头。
利用家里台式机，换了几个配件，搞出了黑苹果。
因为大部分是脚本开发，对性能要求不高，所以配置比较钙。
整体估算下来大概3k左右。性能比官网的6k3 mini钙版还略强。
体验上完全不输mini，某些方面还有超越，比如散热，固态容量。
感谢[@qzz0518](https://github.com/qzz0518/hackintosh_9400f_b360_vega56)的EFI，省了不少事。
有时间再自己研究如何优化配置

## 配件选择
### i3 or i5 or i7
脚本开发，不需要太多核心。
所以CPU追求高频即可。
只考虑入门款，i5 9400F就很尴尬，核心是多两个，频率却比i3低，价格贵一倍，不值。
i7虽好，但是价格……
如果能有效利用多核心，请从i5开始选择。
### 8G or 16G or 32G
mini内存原配8G，真没觉得卡，mac os的高效内存管理+高速固态缓存，体验还是很不错的。
可实在按耐不住骚动的心，自己又花了1K换了两根16G（官网升到32G要+4K4，黑啊），结果发现自己最多只能用到17G……
### 128G or 256G or 512G
mini作为工作机，128G固态真的有点抓鸡，所以黑苹果最好512G或者1T一步到位。
不过手里一块旧的256G，就直接用了。
一定要用m2 nvme的高速固态，这比大内存还管用！！
### 蓝牙
mini就有蓝牙，2.4G，usb 3相互干扰的问题，基本都用有线键鼠。
传文件也都是微信。
对我来说蓝牙就比较鸡肋了，因此就放弃了。
### 显卡
网上有板载HDMI和DVI不能输出的问题，而我又有双显示器的需求。
为了避免不必要的麻烦，就选了独显作为亮机卡。
也不为游戏，入门免驱560即可（其实二手460就行了）。
也不需要视频编码解码，cpu就选了F系列无核显。
### 主板
h310没m2口，不推荐。
b365是上一代马甲。
z390，除非你上k系列cpu超频。
选华硕这块b360板子，是因为有一个type-c口，手里有一些c口的配件。
网上也找到同款EFI，这点很重要。

## 完善程度：
系统版本：macOS Catalina 10.15.3 来源[黑锅小兵的部落阁](https://blog.daliansky.net/macOS-Catalina-10.15.3-19D76-Release-version-with-Clover-5103-original-image-Double-EFI-Version.html) 
SMBIOS：Mac Pro 7.1

* 机箱前置 USB 3.0 接口所有设备正常
* 重启休眠正常
* 主板后置 USB 3.0 接口所有设备正常
* 声卡正常，选内置扬声器。HDMI声音输出也正常。手里还有创新的USB play3声卡，也没问题。
* 显卡 HDMI+DVI 1080p 双显示器
* 更换三码后，AppleId正常使用
* 板载网口正常使用

## 问题
1. 后置TYPE-c
> qzz0518：
> 后置 USB-C 口，只支持 USB 3.1 Gen 1，不支持 USB 2.0 的 USB-C 设备

我手里只有三星X5固态移动硬盘，一切正常。
typc-c的U盘也正常，其他未知

2. 开机内存错误提示
目前选Mac Pro 7.1的通病，无视即可。

## 日志
### 20/02/22 初始配置