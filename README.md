# Fuck Location
[![Stars](https://img.shields.io/github/stars/Mikotwa/FuckLocation?label=Stars)](https://github.com/Mikotwa)
[![Release](https://img.shields.io/github/v/release/Xposed-Modules-Repo/fuck.location?label=Release)](https://github.com/Xposed-Modules-Repo/fuck.location/releases/latest)
[![Download](https://img.shields.io/github/downloads/Xposed-Modules-Repo/fuck.location/total)](https://github.com/Xposed-Modules-Repo/fuck.location/releases/latest)
[![Channel](https://img.shields.io/badge/Telegram-Channel-blue.svg?logo=telegram)](https://t.me/FuckLocation)
[![GitHub license](https://img.shields.io/github/license/Xposed-Modules-Repo/fuck.location)](https://github.com/Xposed-Modules-Repo/fuck.location/blob/main/LICENSE)
[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Mikotwa/FuckLocation/Fuck%20Location%20CI%20Build?label=%F0%9F%9A%80%20CI%20Build&logo=Fuck%20Location)](https://github.com/Mikotwa/FuckLocation/actions)

A simple xposed module that helps you fully control your location.

一个可以帮助你完全控制位置授权的模块

Currently, you may return custom location to specific apps.

目前，你可以对特定的应用返回自定义位置信息。

## Early Alpha version / 早期版本
This module is still in early developement stage. No guarantee whether it will works or not.

该模块处于早期开发阶段。不保证它一定按预期工作。

Targeted in Android 12. Previous versions (like Android 11, 10 and 9) are supported only in theory.

适配 Android 12。以前的版本（如 Android 11、10 或 9）仅仅制作了理论上（即未经真机测试）的支持。

## What's working / 目前已经实现
- Custom WiFi information / 自定义 WiFi 信息
- Custom cell tower information (over LTE / Nr) / 自定义基站信息（LTE 或 Nr 网络制式）
- Custom location provider (like GPS) information / 自定义基于 LocationProvider 返回的位置信息（如 GPS）
- Custom location information coming from requestLocationUpdates / 自定义从 requestLocationUpdates 返回的位置信息

## Plan / 待实现
> ⚠️ DO NOT urge any features that are listed below. They will coming soon in future. / 请**不要**催更下面的特性。它们将在合适的时间到来
- [x] ~~Remove root requirement / 移除对 root 权限的需求~~
- [x] ~~Better app selection page (Search, Organized by alphabets...) / 更好的应用选择页面（搜索、按字母排序...）~~
- [ ] Implement test settings page / 实现设置测试
- [ ] Fix issues that some apps still not working / 修复部分应用仍不能用的问题
- [x] ~~Support custom values of cell tower. / 支持自定义基站的返回值~~
- [ ] Support custom values of WiFi, etc. / 支持 WiFi 等信息的自定义
- [ ] Support individual settings for apps / 支持对应用单独进行设置

## Usage / 使用方法
1. Download & activate this module, then restart. 下载并激活该模块，并重启手机

2. Select applications that you want to take ownership. 选择你想要接管权限的应用

3. Customize the information you want to return to these apps. 设置你想要给这些应用返回的自定义信息

4. That's all. No reboot required. 完成。不需要重启，实时生效。

## Q & A / 常见疑问解答
> After reboot, this module still crash unexpectedly. / 在重启后，模块依然意外闪退。

Look at your log. If anything related to:

*Crash unexpectedly: java.lang.NoClassDefFoundError*

appears, please deactivate all your module (except Fuck Location) temporary and reboot your phone to see if it works.

If it works, then something went wrong on *your* side. Check if any incapable modules were activated.

If it still not work, file an issue.

请查看你的日志。如果有任何类似于：

*Crash unexpectedly: java.lang.NoClassDefFoundError*

的字样，请先临时禁用除 Fuck Location 以外的模块，并重启手机。

如果它能正常运行，问题出在*你*这里。请检查所有潜在的不兼容的模块。

如果依然出现崩溃问题，请发 issue。

> Will this module implement mock location? / 该模块是否会适配模拟位置信息？

No. It is too easy to be detected. / 不会。它太容易被检测到了。

> About cell tower information? / 关于基站信息？

Do NOT ask us. Find for yourself or leave it empty. / 请不要问。有能力自己找，没能力留空。

> Something went wrong on *Fuck Location* side! / Fuck Location 有问题！

Please report this issue with **detailed** logs. / 请携带**详尽**日志文件发 issue。

## Scope / 作用域
You should only select / 你只应选择：
- Android (android)
- Phone (com.android.phone)

Choose anything other than that would not bring you any extra benefits.
选择不是上述的两个应用不会给你带来额外的好处。
