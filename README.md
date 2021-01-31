# EpicMoMiraiG
辅助Mirai进行独立启动，并增加辅助功能 / Help Mirai start independly and add more fuction help Mirai or other programs
## 现有的功能
- 更新Mirai最新源（包含MiraiHTTP，MiraiCore，MiraiConsole，MiraiConsole前端）
- 自动安装并启动Mirai，且无需用户自己操作（相当于一个Mirai自动启动器）
- 自动获取Mirai HTTP的相关信息（ServerIP，Port，Key）
- 颜色区分不同命令
- 日志功能
## 预计加入的功能
- 静默启动（为仅需要QQ发送信息的软件使用）
- 可以自定义配置
- 为每个插件设置独立的更新渠道，可以自动更新（EMG会提供一个下载器）
- 为HTTP开发者直接接入
- 图形化管理插件
等等
## EMG命令（emg [verb][noun]）
 输入emg help以获得帮助
- emg start：开启Mirai
- emg clear: 清空屏幕
- emg getServerIP: 获得HTTP的ServerIP
- emg getServerPort: 获得HTTP的Port
- emg getServerKey：获得HTTP的Key
- emg editServerKey [Value]：自定义ServerKey
- emg fixhttp：修复http占用问题



## 使用方法

1. 打开软件，点击“更新源”
2. 点击“更新”（进入需要点击下载）
3. 输入emg start(报错请重启即可)

## 版本更新

1.0.2:

修复：

- HTTP-API修复逻辑错误
- emg fixhttp逻辑错误
- 部分bugs
- 修改emg 相关处理逻辑
- 修改emg 引用库相关逻辑，使软件运行更快

增加：

- emg stop

1.0.1：

修复：

- 一个可能导致问题的BUG
- 优化内存

加入：

- GUI管理界面
- HTTP-API相关可视化管理

1.0.0：

修复：

- 锁定设置界面
- 修复数组错误
- 修复多开错误

增加：

- HTTP-API修改Key
- 自检

Beta0.3:

- 修复了0.2 Beta的相关Bug
- 更新版本管理
- 优化内置API的处理
  但是，我们仍然发现了一些问题，预计在下个版本修复：
- 数组引用错误
- 多开错误
- EMG关闭逻辑错误
  等等，预计在下个版本会正式供生产环境使用，并且会加入安全模块，这个模块用于辅助程序的安全自检的自我排查问题，优化用户体验

Beta 0.2:

- 修复登录错误逻辑
- 加入对HTTP-api的更多支持
- 画了更多的饼
- 加入账户管理

Beta 0.1:

- 构建EMG核心，暂定为EMG-Core