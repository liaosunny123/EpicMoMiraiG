# EpicMoMiraiG
辅助Mirai进行独立启动，并增加辅助功能 / Help Mirai start independly and add more fuction help Mirai or other programs
# 更快的下载
[EMCloud](http://files.epicmo.cn/?/Github/Package/EpicMoMiraiG/)
**EMCloud下载不会一直为最新的，因为懒，请借助于内置更新检测**
# 插件投稿
在docs文件夹内获得更多信息支持，提交issue即可
## 现有的功能
- 更新Mirai最新源（包含MiraiHTTP，MiraiCore，MiraiConsole，MiraiConsole前端）
- 自动安装并启动Mirai，且无需用户自己操作（相当于一个Mirai自动启动器）
- 自动获取Mirai HTTP的相关信息（ServerIP，Port，Key）
- 渲染与安全
- 日志功能
- 插件中心
- 错误维护
## 预计加入的功能
目前解决完毕，提交issue来帮助开发更过功能
**目前以沫会投入于Linux服务端开发，并行分支均不会再以小版本更新。修复bug发布pre release，大功能(3-5个)发布release**
## EMG命令（emg [verb][noun]）
 输入emg help以获得帮助
(emg help帮助信息不一定为最全的，github帮助文档最全，因为懒)
- emg start：开启Mirai
- emg clear: 清空屏幕
- emg getServerIP: 获得HTTP的ServerIP
- emg getServerPort: 获得HTTP的Port
- emg getServerKey：获得HTTP的Key
- emg editServerKey [Value]：自定义ServerKey
- emg fixhttp：修复http占用问题
- emg stop：终止mirai运行(DEBUG的好方法)
- emg restart：重启mirai
- emg setQQ [QQ]：设置内置管理账号的QQ(限制单个)
## 使用方法
1. 打开软件，点击“更新源”
2. 点击“更新”（进入需要点击下载）
3. 输入emg start(报错请重启即可)
## 版本更新
<<<<<<< HEAD

**2.0.0**

修复

- jre32位下载地址错误
- 删除jre32在菜单栏的提示
- 禁用自行更改菜单栏屏蔽区块代码
- 修复DLL导入后缀不正确的问题
- 修复Json导入不正确的问题
- 修复版本编号问题

增加

- Downloader支持压缩包下载启用

禁用

- 由于版本关系发生变化以及旧版本的不稳定，已禁止版本编号<=2的程序运行，迟于最新版本5个编号的软件运行

注意

若要修改屏蔽区块代码，请在\MConfig\SSetings.emg找到Output中BlockCode选项，设置为1即可

=======
>>>>>>> 76ec0406e91a3ecd22c1e8f18c2245d99dde9f84
**1.0.8**
值得注意的是，1.0.8为一个比较重要的版本，建议用户升级本版本作为日常生产使用的版本，本版本有如下特点：

修复:

- 修复所有已知bug

增加：

- Downloader模块（Downloader模块是一个开放的模块，支持不仅限于EMG的请求，任何人可以随意向EMG请求，若要开发请参见docs）
- 辅助下载（包含Libs、Native-Library组件等等）
- 增加对Native的选项卡，EMG将会适配Native相关功能
- Native：插件安装
- Native：错误日志收集
- Native：环境处理
- Native：Library和jre32处理
- 酷Q-DLL的json自动编写
- Downloader模块的请求文件编写
- EMG错误日志自动收集并提示

**1.0.7**

修复:

- source源的不正确安装

增加:

- 支持屏蔽不正常的代码符号

**1.0.6**

增加：

- 滑块验证
- 非强制性提示不会强制性干扰自动化工作流程

**1.0.4-1.0.5**

增加：

- 插件中心

**1.0.3**:

修复：

- 解决目前所有bug

增加：

- 增加启动项(不仅仅支持Mirai，输出于命令框，支持包含emg在内的所有模块)
- 增加软件设置
- 预增加插件中心

**1.0.2**:

修复：

- HTTP-API修复逻辑错误
- emg fixhttp逻辑错误
- 部分bugs
- 修改emg 相关处理逻辑
- 修改emg 引用库相关逻辑，使软件运行更快

增加：

- emg stop

**1.0.1**：

修复：

- 一个可能导致问题的BUG
- 优化内存

加入：

- GUI管理界面
- HTTP-API相关可视化管理

**1.0.0**：

修复：

- 锁定设置界面
- 修复数组错误
- 修复多开错误

增加：

- HTTP-API修改Key
- 自检

**Beta0.3**:

- 修复了0.2 Beta的相关Bug
- 更新版本管理
- 优化内置API的处理
  但是，我们仍然发现了一些问题，预计在下个版本修复：
- 数组引用错误
- 多开错误
- EMG关闭逻辑错误
  等等，预计在下个版本会正式供生产环境使用，并且会加入安全模块，这个模块用于辅助程序的安全自检的自我排查问题，优化用户体验

**Beta 0.2**:

- 修复登录错误逻辑
- 加入对HTTP-api的更多支持
- 画了更多的饼
- 加入账户管理

**Beta 0.1**:

- 构建EMG核心，暂定为EMG-Core
