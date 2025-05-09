<link rel="shortcut icon" type="image/x-icon" href="./favicon.ico">       

![logo](./OpenWrt_Logo.svg)

[**👉放首行这里说明什么？说明这是你必须要清楚的事情**](./Peace&Love/WhatReallyFuckingMatter.md)           
**👉我们已经处在一个AI爆发前夕，编程的问题应该是AI最擅长的了，不要当只会求助大神的阿巴阿巴，善用chatGPT等工具教你解决问题！**

## DIY区

### 编译
* [小白编译入门](./DIY/fishtool.md)（AI纪元已到，大部分编译报错、插件内核日志报错都可以复制发给chatGPT手把手教你解决！）           
* [OpenWrt_demo](https://t.me/openwrt_demo)（伸手党开箱即用，仅支持x64架构，本博客主编译不定期更新）   

### 开发   
* [成神之路](https://forgotfun.org/2018/04/openwrt-training-2018.html) （佐大OpenWrt开发专业培训班）           

## Lean专区        
* [Lean的发布](https://github.com/coolsnowwolf/lede/releases)

## ImmortalWrt专区      
* [ImmortalWrt](./release/ImmortalWrtSource.md)
                 
## 天灵专区                 
* [天灵的频道](https://t.me/nanopi_r2s)

## eSir专区        
* [eSir的高大全、佛跳墙版本](https://t.me/esirplayground)     

## 固件全新安装升级、不保留配置上传升级相关
* [不保留配置上传升级固件](./tips/Upgrade.md)     
* [固件格式说明](./tips/CHOOSE.md) （openwrt固件常见文件格式的选择）     
* [Rufus](https://github.com/pbatard/rufus/releases) （直写固件到U盘/硬盘/TF卡软件，msata接口的硬盘可以购买转接器转接成usb后连电脑上写入固件）       
* [DiskImg](./tips/PEwirteIMG.md)（PE环境下写入固件到硬盘兼容性最好的v1.2版本）        
* [starwindconverter](https://www.starwindsoftware.com/tmplink/starwindconverter.exe) （虚拟机镜像转换）        
* [ImmortalWrt 系统-软件包 安装插件](./tips/JBipk.md)          
* [ipk离线安装的两种常用方法](./tips/JBipk2.md)                     
* [虚拟机+EFI固件安装问题汇总](./tips/VMandEFI.md)            
 
* [网速测速](http://test.ustc.edu.cn/)
* [单线程网速测速](http://speed.cloudflare.com)        
* [梯子网速测速](https://www.speedtest.net/) （请注意先确保此网站被规则代理了）   
* [几种加密算法下传输速度测试脚本](./sh/ss_test.md)        
* [搬瓦工提供IP连通性测试](https://ping.pe)   
* [国内各省市对某网站ping检测](http://ping.chinaz.com)             
* [ip111查询IP地址](http://www.ip111.cn)    
* [skk查询IP地址](https://ip.skk.moe/)             

* [telegram官方下载地址](https://telegram.org/apps)    
* [telegram汉化简体(推荐第三方)](https://t.me/setlanguage/classic-zh)     
* [telegram汉化简体(官方测试版本)](https://t.me/setlanguage/zh-hans-raw)      
* [telegram汉化繁体(官方测试版本)](https://t.me/setlanguage/zh-hant-raw)        
* [禁止telegram垃圾广告群拉我入群](./tips/TGantiADpull.md)    
* [为什么我无法telegram私聊和在公开群发言？？？](./tips/TGchatForbiden.md)
* [下载telegram群文件的正确姿势](./tips/RuHeZhengQueXiaZaiTGFile.md)                      

## 教程区       

### passwall相关        
* [passwall的流程](https://github.com/xiaorouji/openwrt-passwall/discussions/1506#discussioncomment-1751550)
* [关于passwall的DNS问题](./tips/passwallDNS.md)     
* [passwall+smartdns+adguardhome青阳魂推荐方案](https://github.com/luckyyyyy/blog/issues/57)
* [不希望任何人的设备连到我的openwrt路由下都可以翻墙](./tips/NoFriendUSEmyFQ.md)
* [passwall指定特定设备走特定节点](./tips/passwallTeDingSheBeiQuanJuDaiLi.md)          
* [passwall指定特定网站走特定节点](./tips/passwallURLfenliu.md)      
* [passwall指定特定网站走特定节点初次无法使用问题](./tips/passwallURLfenliuFail.md)     
* [BT下载不走代理、翻墙线路极限速率测试、守护进程](./tips/passwallAdvancedSetting.md)                   
* [帮助完善passwall的手动添加规则](./tips/helpPasswallProxyFile.md)    
* 分流配置中的`黑洞`意思是把它的DNS解析请求都返回错误的本机地址，就是主动墙掉这个服务的意思     
* 目前谷歌等浏览器可能会默认开启QUIC协议传输流量，目前来看它并不受到市场的完美兼容，目前不用为好，请保持passwall分流中的QUIC黑洞待遇
* 可以使用负载均衡同样地实现故障切换功能
* 恢复默认配置方法，地址栏输入例：            
```
http://192.168.5.1/cgi-bin/luci/admin/services/passwall/reset_config
```        
* 隐藏菜单方法，地址栏输入例：            
```
http://192.168.5.1/cgi-bin/luci/admin/services/passwall/hide
```         
* 当你隐藏后想再次显示，地址栏输入例：                          
```
http://192.168.5.1/cgi-bin/luci/admin/services/passwall/show
```        
* passwall芝麻开门命令（如果需要开门）：                      
```       
touch /etc/config/passwall_show        
```      

### ssrp相关      
* [ssrp的分流如何开启](./tips/ssrpFenLiu.md)    
* [ssrp的翻墙线路莫名其妙变动](./tips/ssrpXJBbian.md)   
* [ssrp莫名代理本不该走代理的 淘宝、百度 ...](./tips/proxyWrong.md)      
* ssrp芝麻开门命令（如果需要开门）：                   
```
echo 0xDEADBEEF > /etc/config/google_fu_mode
```    

### openwrt-nikki相关
* [这个UP主对Nikki说得很详细](https://youtu.be/sl8zK0dv7iM?si=X9IDK0-D9X5cJLHb)

### 其他插件相关         
* [禁止一些自己用不上插件开机自启](./tips/noAutoLauch.md)
* [关闭openwrt的ipv6](./tips/OFFipv6.md)          
* [tcpdump抓包](./tips/tcpdump.md)     
* [填入字符后保存应用为何不生效](./tips/saveFail.md)
* [后台LuCI页面显示异常报错](./tips/luciViewBUG.md)
* [网关代理"旁路由"相关](./tips/PangLuYouGNM.md)       
* [LuCI21.02的多LAN口设置在哪里](./tips/luci21.02.md) 
* [upnp相关问题整理](./tips/upnp.md)    
* [NAT路由类型检测工具NatTypeTester](https://github.com/HMBSbige/NatTypeTester/releases)                            
* [手动挂载移动硬盘/U盘](./tips/ManullyGuaZai.md)         
* [web界面操作的超简单DDNS-GO解析IPV4\IPV6到域名](./tips/ddnsGO.md)
* [动态DNS中配置阿里云DDNS](./tips/ddns.md)
* [看一下是否需要打开外网访问路由后台](./tips/webadmin.md)           
* [最强文件分享服务器FileBrowser](./tips/FileBrowserNB.md)         
* [纯命令行交互百度网盘第三方客户端程序](./tips/biaduPCS-Go.md)
* [挂在路由上的百度网盘客户端](./tips/BaiDuWangPan.md) (baidupcs-web开发姐姐已经跑路了)             
* [家里自建一个ssr服务端](./tips/ssrMDBServer.md)       
* [WAN口丢失后重建](./tips/CreWAN.md)      
* [WAN口灯不亮/WAN口无网络连接](./tips/WANfail.md)      
* [自定义登陆界面背景](./tips/argonPic.md)      
* [在openwrt上使用Samba协议打造家庭影音库](./tips/sambaNB.md)             

## 其他区 
* [清理windows系统下DNS缓存](./tips/clearDNS.md)        
* [关闭浏览器的QUIC协议](./tips/killQUIC.md)
* [路由下主机数据传输速率查看](./tips/HostSpeedMonitor.md)     
* [系统资源消耗实时监控查看](./tips/CPUandRAMmonitor.md)     
* [检测ax6/ax3600的真实时钟频率](./sh/clockHz/ax6&3600clockHz.md)         
* [日志粘贴分享网站避免直发群内刷屏](https://paste.debian.net/)
* [banner生成器](http://www.network-science.de/ascii)        
* [ip反查绑定过的域名](https://tools.ipip.net/ipdomain.php)      
* [GitHub各项服务状态](https://www.githubstatus.com)     
* [主流网站的可用状态](https://downdetector.com)      
* 强制转换浏览器页面暗黑Edge拓展插件 [DarkReader](https://microsoftedge.microsoft.com/addons/detail/dark-reader/ifoakfbpdcdoeenechcleahebpibofpc) （人道主义提示，请在访问此类网站时暂时手动关闭此插件：考试、银行、前端调试、素材库...）    
* [在windows电脑上安装emby服务端+百度网盘 的自建影音库方案](./tips/embyINwin.md)
* [Ubuntu18桌面版影音服务器](./tips/Ubuntu18Desk.md)
         
## 常用命令、操作区         
* openwrt关机（再开机需要拔插电源线）
```   
poweroff 
```        
* 忽略依赖报错强行安装某ipk             
```
opkg install --nodeps luci-app-autoreboot
```
* 完全删除lede文件                
```
rm -rf lede
```           
* 清空回收站                                 
```
sudo rm -rf ~/.local/share/Trash/*
```         
* Windows的HOSTS文件位置(当出现一些网页元素加载失败时可以尝试清空HOSTS规则)               
```
C:\Windows\System32\drivers\etc
```         
* powershell中SSH连接路由器后台举例                 
```
ssh root@192.168.2.1
password
```         
* openwrt恢复出厂设置命令                      
```
firstboot
```          
* 修改LAN口IP                       
```
vi /etc/config/network
i
:wq!
```             
* 默认root进入系统后添加普通用户          
```
sudo useradd -m zhangsan -s /bin/bash
sudo passwd zhangsan
sudo adduser zhangsan sudo
su zhangsan
cd /home/zhangsan
sudo apt-get update
sudo apt-get install vim
```                   
* 举例指定git拉取my-19.07分支           
```
git clone -b my-19.07 https://github.com/Lienol/openwrt.git
```                
* 显示隐藏文件（.config）          
```
ls -a 
```     
或 
Ctrl+H                
* git冲突，放弃本地修改，直接覆盖                    
```
git reset --hard
git pull
```            

## 启示录区       
* [万兆无线路由器，真的能跑万兆无线网吗？](https://sspai.com/post/71581)                             
——少数派           
`* 远离二道宽带贩子，优选 电信/联通 > 移动 > 其他`      
`* 换同端口速率的光猫基本没什么卵用，不是决定性因素`       
`* 买一个高性能的路由器比什么都重要，新购路由优选 ARM > MIPS,翻墙去广告QOS有需求请尽量选择x86`        
`* 如果想要家中每个角落都能享受到好的信号，优选多个无线AP错开信道，再不行就上电力猫，无线桥接候选`        
`* 无线穿墙性能其实取决于双方，对，你的接收端，例如手机`            
`* 尽量远离MTK，抗干扰选择 QCA/AR，覆盖选 BCM`         
`* 基本没有第三方的无线性能会比原厂更好`     
`* 家里尽量不要用二级路由，普通路由接LAN口关闭DHCP服务即可做AP，或者打开AP模式`         
`* HWNAT 对小包（小于 128K) 不会有加速效果，而大部分游戏和 DNS 等都是小的 UDP 报文，这时候都靠 CPU 转发，x86 软路由有明显的转发性能优势`         
`* 挨个检查客人手机里是否装了WiFi万能钥匙，发现的立马打死`        
——Lean的QQ群：297253733                                              
`* 有很多人天天都在焦虑，怕没得到，怕寂寞`        
——《士兵突击》                
*佐大30岁的人生感悟*        
  *虽然我的人生充满了苦难，但一眨眼就到了30。30后，感觉自己变得更念旧和无力，因为自己已不再辉煌，所以一直追忆着25岁的自己。虽然知道这样无济于事，但是人毕竟需要一个心灵的慰藉，无论是真是假、是虚是实。       
  在大学时，我曾自诩是一位很有"思想"的人，对身边的人暗生讥讽，认为自己高人一等。现在看来，当年的我是多么的无知和不可一世，"独立思考”的人格谈何容易，很多时候我们只是父母思想的映射，如同提线木偶。我们的一言一行、一举一动都是父母长期影响下的结果，实际上只是父母思想的一部分拷贝。虽然决定来自于你自己的大脑，但思维模式没有跳出你父母的条条框框。   
  这么多年来，我一直犯了一个错误。过度批判和抵制古典文学，错过了古人留给我们的瑰宝。现在看来，西方哲学只是古典文学的子集，不得不惊叹古人的智慧。                
  每个人的心中都藏着一位梦中情人，无数的夜晚我们还会因彼此未能成就姻缘而黯然泪下。现在看来，那只是徒增伤悲罢了，因为一旦分离已注定此生再无交集，既无此生何谈来世。人生就向一辆永不停歇的火车，既然已在岔口分离，那彼次只会渐行渐远。她喜欢的是你，是当年的你。你喜欢的她，是当年的她。事过境迁，彼此早已不在是当年的自己。"两情若是久长时，又岂在朝朝暮暮"在我看来，描述的是亲情，而非爱情，似乎很多人都误解了，包括我自己。           
  以前的我，表现地与世无争。现在看来，只是懦弱和无能的表现而已，并没有高尚到哪里去。在人的生存空间越来越受挤压的当下，你自己不去拼命争取没有人会帮你保留空间。这个世界就是那么残酷，你的敌人在宣告胜利的同时，还不忘给你滋上一泡尿。更令人痛心的是，提出滋你一身的人，恰好是你当年的"梦中情人"。人性这东西，是你一辈子都看不明白、琢磨不透的。           
  以前的我，遇到挫折和失败就会陷入过度自责中、反省当初的自己。现在看来，挫折和失败的隐患早在你出生时就已埋下，你所遭遇的挫折和失败只是爆发后的结果。你若不从根本上拔除身上的祸根，未来的你还会遭遇同样的惨剧。你还会因为不善于交际而吃人事的亏，你还会因为不善于搭讪而缺女人缘，你还会因为不懂人情世故而遭人排斥，悲剧还会一次次重演。*           
——佐须之男          

## 友链       
* [青阳魂的博客](https://williamchan.me/)     
* [Padavan路由固件](https://opt.cn2qq.com/)          

## About   
* 作者的 [微博账号](https://weibo.com/yangmiblog)          
* 提示：如果部分页面含有的教程图片较小无法正常阅读有效信息，请短暂放大网页即可(手机端两指拉伸/PC端Ctrl+滑轮上划)       
