# 前言

本文档旨在帮助你了解EMG的source相关的信息，你可以在阅读本文档后利用EMG内置的下载器完成你自己的更新需要

EMG中，更新被定义为“更新源”+“更新”，其中更新源只是简单的更新这些链接文件的地址，而不会真正的更新，这个操作可以给更多的插件加入到某一次更新的更新源

## 更新原理

EMG的更新包含如下方案：更新源+更新

更新源：单独更新某个源文件的指向的链接

更新：执行真正的更新操作

为什么这么做？

这样做方便了程序的统一更新和管理，避免很多插件自己更新而造成的需要不断的reload和重启，同时便于规范

我需要做什么？

提供更新源的指向即可，更新由EMG的子模块Downloader执行，Downloader会托管更新并且支持多种下载方案

更新模式（V1.0.2-）？

> 由于时间原因，暂时无法单独拿出Downloader子模块，只能在原Source的基础上进行二次开发，原逻辑仅限于Source

> 应当注意的是，我们在DLinks里面目前仅接受蓝奏云的链接

提供DFiles、DLinks、DFrom、DTask

你应当按照配置项格式编写，详情可见MConfig\source.emg，你需要单独建立一个DFrom并提供Author，Version，Describe三个内容，其余仿照即可，建立后将你的文档提供给Source.emg即可

## 插件投稿
Name=插件名称
FilesName=插件保存文件（带后缀）
Describe=（一句话描述）
Version=插件版本
EMGVersion=1
Github=项目地址
LZLinks=
Able=True
Time=日期
e.g.
Name=EMG-Test
FilesName=EMG-Test.jar
Describe=EMG测试插件
Version=1.0.0
EMGVersion=1
Github=xxx
LZLinks=
Able=True
Time=2021.2.2
