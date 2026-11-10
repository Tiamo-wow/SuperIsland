# SuperIsland（超级岛）

面向 HyperOS 4 的 LSPosed 模块，提供超级岛解锁动画、应用锁动画和锁屏外观设置。

[下载与版本记录](https://github.com/Tiamo-wow/SuperIsland/releases) · [反馈问题](https://github.com/Tiamo-wow/SuperIsland/issues)

本仓库用于发布 APK、更新说明和收集反馈，暂不提供模块源码。首个公开版本正在准备中，当前尚无 APK 可供下载。

## 功能

- 人脸、指纹和凭据解锁的超级岛动画。
- 应用锁超级岛显示，以及中岛与超级岛组合显示。
- 超级岛宽度、图标位置和解锁后保留时长调节。
- 锁屏 PIN 柔光玻璃键盘、滑动输入及壁纸模糊设置。
- 日志筛选与导出、主题切换和桌面图标开关。

具体功能、已知问题和设备验证范围以对应版本的 Release 说明为准。

## 使用条件

- HyperOS 4，以及支持本模块的 Root／LSPosed 环境。
- 不同 ROM 构建的内部结构可能不同；其他系统版本和设备组合仍需单独验证。
- 模块通过运行时挂接工作，不替换原始系统 APK。

## 安装和启用

1. 在 [Releases](https://github.com/Tiamo-wow/SuperIsland/releases) 下载需要的版本，选择 `.apk` 附件安装。
2. 在 LSPosed 中启用 SuperIsland，并选择以下作用域：

   | 功能范围 | 包名 |
   | --- | --- |
   | 系统界面 | `com.android.systemui` |
   | 系统界面插件 | `miui.systemui.plugin` |
   | 应用锁所需的安全中心 | `com.miui.securitycenter` |

3. 打开模块，阅读首次使用说明，再开启模块及需要的功能。
4. 按页面提示重启系统界面或安全中心，使相应设置生效。

更新前先阅读版本说明。若安装时提示签名不一致，通常需要记录设置后卸载旧包再安装；卸载会清除应用设置。

## 异常恢复

出现异常时，先在 LSPosed 中禁用本模块，再重启相关进程或设备。不要同时启用处理相同行为的旧 DEX 补丁，以免重复修改系统界面行为。

## 反馈问题

请在 [Issues](https://github.com/Tiamo-wow/SuperIsland/issues) 中提供模块版本、ROM 版本、复现步骤和必要的脱敏日志。设备安装、模块挂接和真实功能验证是不同环节，请说明具体在哪一步出现问题。

## 许可

本仓库中的说明文档采用 [MIT 许可证](LICENSE)，Copyright (c) 2026 Tiamo-wow。

该文档许可不构成对 APK 整体的 MIT 授权，也不表示模块源码已公开。APK 中的第三方内容保留各自的许可声明。
