# Netviso（网络透镜）安卓版下载

网络透镜 · 看清你的网络

这里提供 Netviso 安卓公测版安装包、校验文件和更新说明。应用源码不在此仓库公开。

## 下载

当前版本：**0.8.0 build 5（公测版）**，包名 `com.kaka.netviso`。

- [GitHub 下载页](https://github.com/kakadiary/NetViso-Downloads/releases/tag/android-v0.8.0-build5)：在附件（Assets）中下载 `Netviso-0.8.0-build5-android.apk` 和 `SHA256SUMS`。
- [百度网盘镜像](https://pan.baidu.com/s/1yh5OgoWZhq19_4xP9nVZkQ?pwd=58PB)，提取码：`58PB`。镜像继续保留；当前网盘 APK 尚未重新下载核验，请按下面的 SHA-256 自行核对。

## 安装与覆盖升级

适用 Android 10 及以上。下载 APK 后点开安装，按系统提示允许当前浏览器或文件管理器安装应用。

已安装此前正式公测包（包名 `com.kaka.netviso`）的用户，请直接覆盖更新，保留本地检测记录和设置。build 5 与 build 2 使用相同签名证书。不要先卸载，卸载会删除本地数据；如提示签名冲突，请先核对原应用的来源，不要通过卸载强行升级。已安装更高 build 的用户请勿降级。

开发包 `com.kaka.netviso.dev` 与公测包可以共存，检测记录和设置不互通。

这份公测 APK 在系统中仍显示为“Netviso 开发版”。已核对其包名为 `com.kaka.netviso`、调试标志关闭，且使用正式发布签名；本次保持已验收原包不变。

## 本版更新

改善部分 Wi-Fi 环境下检测后的连接复查：备用端口首次预热超时且剩余时间足够时，会补试一次。只有两项后续检查都通过，才按原有规则判断 NAT 类型。检测无法确认时仍保留未确认状态。

## 文件校验

APK SHA-256：

```text
8ad69f676f6e72789f45b7e181c82a0a4f8ed5e488fb0bac35e060d5d27f1f20  Netviso-0.8.0-build5-android.apk
```

将 APK 与 `SHA256SUMS` 下载到同一目录后，可在 macOS 终端运行：

```sh
shasum -a 256 -c SHA256SUMS
```

Linux 使用 `sha256sum -c SHA256SUMS`。Windows PowerShell 使用以下命令，将输出与上面的值逐字比较：

```powershell
Get-FileHash .\Netviso-0.8.0-build5-android.apk -Algorithm SHA256
```

签名证书 SHA-256（与文件校验值不同）：

```text
1c57848b1a7113f6412696d5ce61cd3b2a3dd986f1c293e0aa1ede32ec718b5c
```
