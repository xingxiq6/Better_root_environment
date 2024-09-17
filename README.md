# For Englist User
### Why not write in English? Because there are hardly any English-speaking users, and my English is very poor.

# !!!警告, 免责声明

本安装器不会对您的设备造成的任何后果负责,请自行考虑是否使用

# 更好的root环境 一个帮助快速的配置用户root环境的安装器模块

# XXX检测软件过不去?

##### 本安装器模块是为了更好的节省隐藏的时间, 解决大部分app打不开的问题. 而不是为了过检测而设计, 帮助作弊用户等等

# 安装需求
### Android版本8.1+<sup>*必须</sup>
### Android版本10+<sup>*推荐</sup>
### 内核版本号4.9+<sup>*推荐</sup>
### Apatch 10865或10884, KernelSU_v1.0.1, Magisk Alpha 27007 或 Magisk Alpha 27007 (不推荐用Magisk Delta)<sup>*推荐</sup>

# 安装方法

### 前置要求
##### 手动前往github下载对应版本的 Zygisk Next 和 Tricky Store 并放入对应压缩包文件夹内
##### 1.将Zygisk Next放在压缩包的/modules文件夹内并改名为sha256的文件名
##### 2.将Tricky Store放在压缩包的/modules/android10+文件夹内并改名为sha256的文件名

### 安装流程
##### 1.下载最新模块, 并完成前置要求
##### 2.保证/data/adb文件夹是干净的 <sup>*推荐</sup>(改名重启即可)
##### 3.安装最新模块
##### 4.手动导入最新生成的/sdcard/hma.json文件并进行相应的配置. 按照模块状态进行重启手机1~2次
##### 5.享受模块带来的便利吧!!!

# 中国网盘克隆链接<sup>*更新不及时, 不推荐</sup>

### 蓝奏云
##### [https://wwie.lanzoub.com/b0nyeec8b?pwd=root#root]
##### 密码: root

# 发现问题?

##### 请发起一个 issues 让我知道(不接受小白问题,比如XXX软件过不去)

## 这个模块做了以下操作

系统模块部分:

1.尝试安装Zygisk-Next-1.1.0[https://github.com/Dr-TSNG/ZygiskNext/releases/tag/v1.1.0]
解决牛头人发现注入的问题

2.安装PlayIntegrityFix-17.5[https://github.com/chiteroman/PlayIntegrityFix/releases/tag/v17.5]
隐藏部分bootloader解锁痕迹,并辅助通过Google SafetyNet

3.安装LSPosed1.8.0[https://github.com/LSPosed/LSPosed/releases/tag/v1.8.0]</br>
3.安装LSPosed-npm-v7075_zygisk-cli(添加lsposed_mod的cli功能)<br></br>
!(来自5ec1cff的Lsposed open npm改编)[https://github.com/5ec1cff]
解决牛头人邪恶服务(2)的问题,并用于激活隐藏app列表Xposed插件模块

4.安装safetynet-fix-v2.4.0_MOD[https://github.com/kdrag0n/safetynet-fix]
为安卓10以下伪装不支持硬件级秘钥认证(安卓10+自动禁用)</br>
4.安装Tricky-Store
伪装bl未解锁,默认将秘钥文件注入所有个人安装app,如有需要请修改自动配置列表模块
[https://github.com/5ec1cff/TrickyStore/releases]

5.安装sui-zygisk-v13.5.1[https://github.com/RikkaApps/Sui/releases/tag/v13.5.1]
默认禁用,未来备用

6.安装Shamiko-v1.1.1[https://github.com/LSPosed/LSPosed.github.io/releases/tag/shamiko-357]
隐藏大部分root痕迹(APatch用户不安装,请手动安装cherish_peekaboo_1.4.2.kpm)

7.安装SelinuxHide </br>
默认不启用防止暴露更多root痕迹
可能可解决momo提示隐藏selinux为宽容模式，seccomp未开启，init.rc被修改，处于调试环境，art参数异常，非sdk的链接限制失效

8.安装自动配置辅助模块, 实现自动更新app注入列表

apk部分:
1.安装爱玩机工具箱S-22.0.9.3及其辅助插件

2.安装第三方酷安c001apk_540265e[460]

3.安装改包名版隐藏应用列表v3.2
解决牛头人邪恶服务(1)的问题, 并隐藏部分app列表

4.安装破解MT管理器及其附属终端

细节操作

1.自动释放已配置的LSPosed模块作用域

2.自动生成预配置黑名单的隐藏应用列表[https://github.com/5ec1cff/Hide-My-Applist/blob/master/README_zh_CN.md]配置文件到/sdcard的hma.json文件中