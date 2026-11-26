# Netviso（网络透镜）安卓版下载

网络透镜 · 看清你的网络

这里提供 Netviso 安卓公测版安装包、校验文件和更新说明。应用源码不在此仓库公开。

## 下载

当前 GitHub 下载版本为 **0.8.0 build 6（公测版）**，包名 `com.kaka.netviso`。

- [GitHub 下载页](https://github.com/kakadiary/NetViso-Downloads/releases/tag/android-v0.8.0-build6)。在附件（Assets）中下载 `Netviso-0.8.0-build6-android.apk`、`SHA256SUMS` 和「安装必读」。
- [夸克网盘镜像](https://pan.quark.cn/s/f668cac4a6b7?pwd=GtRm)，提取码：`GtRm`。
- [百度网盘镜像](https://pan.baidu.com/s/1yh5OgoWZhq19_4xP9nVZkQ?pwd=58PB)，提取码：`58PB`。镜像版本以网盘页面为准。下文校验值对应 GitHub 上的 build 6 APK。

## QQ 交流群

群号：**1047103574**。欢迎交流使用体验、反馈问题和建议。

## 安装与覆盖升级

适用 Android 10 及以上。下载 APK 后点开安装，按系统提示允许当前浏览器或文件管理器安装应用。

已安装此前正式公测包（包名 `com.kaka.netviso`）的用户，请直接覆盖更新，保留本地检测记录和设置。build 6 与 build 5 使用相同签名证书。不要先卸载，卸载会删除本地数据；如提示签名冲突，请先核对原应用的来源，不要通过卸载强行升级。已安装更高 build 的用户请勿降级。

开发包 `com.kaka.netviso.dev` 与公测包可以共存，检测记录和设置不互通。

这份公测 APK 在系统中仍显示为“Netviso 开发版”。已核对其包名为 `com.kaka.netviso`、调试标志关闭，使用正式发布签名。

## 本版更新

- 修复新检测得到符合条件的「全锥型 · NAT1」结果时礼花未触发的问题。
- 设置页和结果页统一提供 miwifi、fitauto 两个预设，支持自定义地址。
- 检测记录可按天折叠，支持直接删除单条记录，优化较多记录时的加载速度。
- 改善 Wi-Fi 名称读取，VPN 开启时分别显示 Wi-Fi 和隧道地址。

## 文件校验

GitHub build 6 APK 的 SHA-256（APK 于 2026-11-26 更新）

```text
dbfb40a5fdd3ef5b171e6aed89ad5fdc0f80715668c1099b149912ee210d53f2  Netviso-0.8.0-build6-android.apk
```

将 APK 与 `SHA256SUMS` 下载到同一目录后，可在 macOS 终端运行：

```sh
shasum -a 256 -c SHA256SUMS
```

Linux 使用 `sha256sum -c SHA256SUMS`。Windows PowerShell 使用以下命令，将输出与上面的值逐字比较：

```powershell
Get-FileHash .\Netviso-0.8.0-build6-android.apk -Algorithm SHA256
```

签名证书 SHA-256（与文件校验值不同）：

```text
1c57848b1a7113f6412696d5ce61cd3b2a3dd986f1c293e0aa1ede32ec718b5c
```
