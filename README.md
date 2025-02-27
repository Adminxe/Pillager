# Pillager

[![License](https://img.shields.io/github/license/qwqdanchun/Pillager.svg)](LICENSE)
![GitHub last commit](https://img.shields.io/github/last-commit/qwqdanchun/Pillager)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/qwqdanchun/Pillager)
[![Downloads](https://img.shields.io/github/downloads/qwqdanchun/Pillager/total.svg)](https://github.com/qwqdanchun/Pillager/releases)
![Issues](https://img.shields.io/github/issues/qwqdanchun/Pillager)

<img src=".\Pillager.png"/>

## 介绍

Pillager是一个适用于后渗透期间的信息收集工具，可以收集目标机器上敏感信息，方便下一步渗透工作的进行。

## 支持

| Browser       | BookMarks | Cookies | Passwords | Historys | Local Storage | Extension Settings |
| :------------ | :-------: | :-----: | :-------: | :------: | :-----------: | :----------------: |
| IE            |    ✅    |   ❌   |    ✅    |    ✅    |      ❌      |         ❌         |
| Edge          |    ✅    |   ✅   |    ✅    |    ✅    |      ✅      |         ✅         |
| Chrome        |    ✅    |   ✅   |    ✅    |    ✅    |      ✅      |         ✅         |
| Chrome Beta   |    ✅    |   ✅   |    ✅    |    ✅    |      ✅      |         ✅         |
| Chrome SxS    |    ✅    |   ✅   |    ✅    |    ✅    |      ✅      |         ✅         |
| Chromium      |    ✅    |   ✅   |    ✅    |    ✅    |      ✅      |         ✅         |
| Brave-Browser |    ✅    |   ✅   |    ✅    |    ✅    |      🚧      |         🚧         |
| QQBrowser     |    ✅    |   ✅   |    ✅    |    ✅    |      ✅      |         ✅         |
| SogouExplorer |    ✅    |   ✅   |    ✅    |    ✅    |      🚧      |         🚧         |
| 360ChromeX    |    ❌    |   ✅   |    ✅    |    ❌    |      ✅      |         ✅         |
| Vivaldi       |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| CocCoc        |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Torch         |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Kometa        |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Orbitum       |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| CentBrowser   |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| 7Star         |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Sputnik       |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Epic Privacy  |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Uran          |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| Yandex        |    🚧    |   🚧   |    🚧    |    🚧    |      🚧      |         🚧         |
| FireFox       |    ✅    |   ✅   |    ✅    |    ✅    |      ❌      |         ✅         |

注：✅表示经过测试，🚧表示理论上支持但未经测试，❌表示无此功能或不支持

|    IM    |      Support      |
| :------: | :----------------: |
|    QQ    | ClientKey（Email） |
| Telegram |       tdata       |
|  Skype  |       Token       |
|  Enigma  | DeviceID/Datebase |

|   Tool   |       Support       |
| :-------: | :-----------------: |
| MobaXterm | Password/Credential |
| Xmanager |      Password      |
|  Navicat  |      Password      |
|  RDCMan  |      Password      |

|    Mail    | Support |
| :--------: | :------: |
| MailMaster | DataFile |

| Others | Support |
| :----: | :------: |
|  Wifi  | Password |

后续将会陆续添加支持的软件

## 使用方法

此项目使用Github Action自动编译打包，并上传至[Release](https://github.com/qwqdanchun/Pillager/releases)，其中

* [Pillager.exe](https://github.com/qwqdanchun/Pillager/releases/download/AutoBuild/Pillager.exe) 为.Net Framework v3.5编译生成的exe
* [Pillager.bin](https://github.com/qwqdanchun/Pillager/releases/download/AutoBuild/Pillager.bin) Donut打包的raw格式的shellcode
* [cs-plugin.zip](https://github.com/qwqdanchun/Pillager/releases/download/AutoBuild/cs-plugin.zip) 为适用于CobaltStrike使用的插件

使用CobaltStrike可以直接下载插件包，其他人推荐将shellcode集成至自己的加载器或工具中运行，不建议直接使用Pillager.exe

执行后会将文件打包至 `%Temp%\Pillager.tar.gz`，需要自行前往目录下载文件或修改代码将文件上传至他处

## 优点

* 体积在100kb左右，为同类工具体积的几分之一甚至几十分之一
* 支持大部分常见浏览器，常见聊天软件的信息提取，将陆续添加其他常用工具的信息收集
* 长期维护，有问题可以及时的反馈处理
* 使用魔改版本的Donut，缩小shellcode体积，使shellcode兼容.Net Framework v3.5/v4.x，并去除AV/EDR对Donut提取的特征

## Contributors

<a href="https://github.com/qwqdanchun/Pillager/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=qwqdanchun/Pillager" />
</a>

## 404星链计划

![](https://github.com/knownsec/404StarLink-Project/raw/master/logo.png)

Pillager 现已加入 [404星链计划](https://github.com/knownsec/404StarLink)
