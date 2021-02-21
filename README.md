# AutoBuild-OpenWrt
[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat&logo=github&label=LICENSE)](https://github.com/esirplayground/AutoBuild-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/esirplayground/AutoBuild-OpenWrt.svg?style=flat&logo=appveyor&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/esirplayground/AutoBuild-OpenWrt.svg?style=flat&logo=appveyor&label=Forks&logo=github)
![GitHub last commit](https://img.shields.io/github/last-commit/esirplayground/AutoBuild-OpenWrt?label=Latest%20Commit&logo=github)

使用GitHub Actions构建OpenWrt固件精益的OpenWrt，
特此感谢P3TERX的出色工作：https://github.com/P3TERX/Actions-OpenWrt/

在此，感谢KFERMercer所做的出色工作：https://github.com/KFERMercer/OpenWrt-CI
您可以编辑并启用“同步代码” YAML文件，以使您的分叉存储库保持更新。

感谢eSir所做的出色工作：https://github.com/esirplayground/AutoBuild-OpenWrt

用法
1.前提条件

注册GitHub动作
分叉此GitHub存储库
2.编译固件

单击[.github/workflows]仓库顶部的文件夹，您会看到很少的工作流文件，每个文件用于一个特定的体系结构（设备）。
编辑所需的工作流文件，取消注释将第3行挤在一起并提交提交。（其他2种方法等待您发现）
构建将自动开始。可以在“操作”页面上查看进度。
构建完成后，单击Artifacts“操作”页面右上角的按钮以下载二进制文件。
默认的Web管理员IP 192.168.5.1：，用户名root，密码password
3.同步码

取消注释“ push-branches-master”On部分下的3行，并提交更改，以使脚本一次为您同步代码。
取消注释“ schedule-cron”两On节，并提交更改以使脚本每天凌晨3点同步代码[UTC +8]
有关详细信息，请访问我的Y2B频道（中文）| 视频教程(https://www.youtube.com/c/esirplayground)
