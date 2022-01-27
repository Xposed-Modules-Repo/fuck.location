# FuckLocation
[![Stars](https://img.shields.io/github/stars/Mikotwa/FuckLocation?label=Stars)](https://github.com/Mikotwa)
[![Release](https://img.shields.io/github/v/release/Xposed-Modules-Repo/fuck.location?label=Release)](https://github.com/Xposed-Modules-Repo/fuck.location/releases/latest)
[![Download](https://img.shields.io/github/downloads/Xposed-Modules-Repo/fuck.location/total)](https://github.com/Xposed-Modules-Repo/fuck.location/releases/latest)
[![Channel](https://img.shields.io/badge/Telegram-Channel-blue.svg?logo=telegram)](https://t.me/FuckLocation)
[![GitHub license](https://img.shields.io/github/license/Xposed-Modules-Repo/fuck.location)](https://github.com/Xposed-Modules-Repo/fuck.location/blob/main/LICENSE)

A simple xposed module that helps you fully control your location.

一个可以帮助你完全控制位置授权的模块

Currently, you may return custom location to specific apps.

目前，你可以对特定的应用返回自定义位置信息。

## Early Alpha version / 早期版本
This module is still in early developement stage. No guarantee whether it will works or not.

该模块处于早期开发阶段。不保证它一定按预期工作。

Targeted in Android 11 - 12. Previous versions (like Android 10 and 9) are supported only in theory.

适配 Android 11 及 12。以前的版本（如 Android 10 或 9）仅仅制作了理论上（即未经真机测试）的支持。

## What's working / 目前已经实现
- Custom WiFi information (only in Android 11+) / 自定义 WiFi 信息（仅 Android 11+）
- Custom cell tower information (over LTE, only in Android 11+) / 自定义基站信息（LTE 网络制式，仅 Android 11+）
- Custom location provider (like GPS) information / 自定义基于 LocationProvider 返回的位置信息（如 GPS）

## Usage / 使用方法
> ⚠️ This module require root to sync your settings. Grant the permission if asked. 该模块需要 root 权限来同步设置。如果你看到授权请求，请同意。

1. Download & activate this module, then restart. 下载并激活该模块，并重启手机

2. Select applications that you want to take ownership. 选择你想要接管权限的应用

3. Customize the longtitude & latitude you want to return to these apps. 设置你想要给这些应用返回的自定义经纬度

4. That's all. No reboot required. 完成。不需要重启，实时生效。

## Scope / 作用域
You should only select Android Framework. 你只应选择 Android 框架。
