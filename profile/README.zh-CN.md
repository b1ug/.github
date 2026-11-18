# blink(1) 爱好者社区

为 [blink(1) USB 灯](https://blink1.thingm.com/) 构建易用的软件。
我们是独立用户社区，不是硬件制造商。

[English](README.md)

## 从 nb1 开始

[安装 nb1 并打开本地工作台](https://b1ug.github.io/nb1-docs/zh/getting-started)。
同一个原生程序提供 CLI、可选 daemon 与内嵌 Web；匹配的 MCP adapter 与 Agent Skill
是可选下载。

## 选择对应的项目

| 项目 | 用途 |
| --- | --- |
| [nb1](https://github.com/b1ug/nb1) | 原生 CLI、daemon、HTTP API、设备所有权和本机存储。 |
| [nb1 Documentation](https://github.com/b1ug/nb1-docs) · [文档站](https://b1ug.github.io/nb1-docs/zh/) | 英中安装教程、API 与 Agent 示例；静态页面不访问 USB。 |
| [nb1 Embedded Workbench](https://github.com/b1ug/nb1-workbench) | 编译进 nb1 的前端源码，通过 `/demo/` 调用本地 daemon 的 HTTP API。 |
| [nb1 Browser Tools](https://github.com/b1ug/nb1-browser-tools) | 独立 WebHID 开发预览与实验性 Chrome 提醒扩展，直接持有 USB。 |
| [Homebrew tap](https://github.com/b1ug/homebrew-tap) | macOS/Linux 源码安装，服务由 `nb1 service` 显式管理。 |
| [blink1-go](https://github.com/b1ug/blink1-go) | blink(1) Go SDK，提供设备命令、解析与能力信息。 |
| [GID](https://github.com/b1ug/gid) | 原生应用的 Go USB HID 访问库。 |
| [colorkit](https://github.com/b1ug/colorkit) | 可复用的纯 Go 颜色类型、CSS 名称、Hex 与 HSV 转换。 |

内嵌工作台与 Browser Tools 是不同入口。另一控制者打开同一只灯前，先停止或断开
当前控制者。Browser Tools 不安装原生 daemon；文档站不控制设备。安装前应查看对应
仓库的发布状态与支持范围。

Go module 提供 Go 代码；独立维护的内嵌前端以固定源码和逐文件哈希导入，普通 nb1
构建不需要 Node 或递归检出 submodule。

## 参与

在对应仓库反馈问题、改进文档或提交提案。正式版、开发预览和规划 API 分开标示。
硬件支持记录实际型号、系统和验收范围；屏幕预览与缓存 RGB 不代表光学测量。
