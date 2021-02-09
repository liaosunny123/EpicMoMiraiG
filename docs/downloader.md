# 前言

本文档旨在帮助你了解EMG的downloader相关的信息，你可以在阅读本文档后利用EMG-Downloader模块完成插件下载工作

# 使用

EMG中采用文件传递的方式启用Downloader（版本编号2，区别于Source\Download模块)，此模块不同于Downloader模块，他支持：

- Lanzou
- LanzouZIP
- Normal

编写格式：

[Task]

//任务数量

Number=1

//类型

Type=Normal
[Durl]

//不同的下载地址

1=url
[DFiles]

//保存的相对路径，以EpicMoMiraiG所在的目录作为根目录

1=\jre32.msi

注：Lanzou和LanzouZIP会自动解析，ZIP会自动解压到zip所在目录，保存地址应该有后缀名，此外，请覆盖\MConfig\downloader.emg并call Downloader窗口完成下载

编辑于：2021.2.9 (EMG:v2.0.0)

