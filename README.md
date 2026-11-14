# Clash for Young

一个新手也能自己装好、用好的代理客户端：**粘贴订阅、点连接、给网站选地区**。

基于 [mihomo](https://github.com/MetaCubeX/mihomo) 内核，支持 Mac 和 Windows，使用 Clash 格式订阅。

## 功能

- **上手简单**：粘贴订阅链接就能用，点小猫连接 / 断开（睡着 = 未连接，睁眼 = 已连接）
- **按网站选线路**：AI、视频、社交、科研等常用网站可以各自选择直连、某个地区或某个节点，也能添加自己的网站和规则
- **节点自动分组**：多个订阅合在一起，按地区自动归类，可自定义
- **增强模式（TUN）**：可选，让终端、游戏等不走系统代理的程序也走代理
- **同步到手机**：一键导出配置，导入 iPhone 的 Clash Mi 或安卓的 FlClash / Clash Meta for Android
- **省心可靠**：国内网站始终直连、DNS 不泄漏，订阅自动更新，软件一键更新，退出或崩溃后自动恢复网络

## Pro 版

需要更强大、更专业的功能？可以联系我获取 **Pro** 版和 **WRT Pro** 版（适用于 OpenWrt）：📧 annoying-hut-vowel@duck.com

## 下载安装

在 [Releases](../../releases) 下载：

| 系统 | 文件 |
|---|---|
| Mac（Intel 和 Apple 芯片通用） | `clash-for-young_版本号_universal.dmg` |
| Windows | `clash-for-young_版本号_x64-setup.exe` |

**Mac**：打开 `.dmg`，把 Clash for Young 拖进「应用程序」。没有苹果开发者签名，第一次打开会被拦截：

- 提示“无法验证开发者”：到「系统设置 → 隐私与安全性」点「仍要打开」
- 提示“已损坏”：在终端执行 `xattr -dr com.apple.quarantine "/Applications/Clash for Young.app"`

**Windows**：运行安装程序；出现 SmartScreen 提示点「更多信息 → 仍要运行」。
如果杀毒软件提示 `mihomo.exe` 有风险（代理内核常被误报），请在杀毒软件里恢复它并把安装目录加入白名单。

## 万一断网

软件正常退出时会自动关闭系统代理。如果软件被强制结束后上不了网，重新打开 Clash for Young 会自动恢复；或者手动关闭系统代理：

- Mac：系统设置 → 网络 → 当前网络 → 详细信息 → 代理，关掉所有勾选
- Windows：设置 → 网络和 Internet → 代理 → 关闭「使用代理服务器」

## 分流规则

从上到下依次匹配：

1. 自定义规则（高级）
2. 网站页里单独设置过的网站
3. 预设规则（内网、国内网站直连）
4. 其余 → 首页选的默认地区

订阅里自带的规则不使用，只用它的节点。

## 许可证

GPL-3.0。mihomo 内核同为 GPL-3.0。
