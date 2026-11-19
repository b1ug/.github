# blink(1) user group

Community software for the [blink(1) USB light](https://blink1.thingm.com/).
We are an independent user group, not the hardware manufacturer.

[简体中文](README.zh-CN.md)

## Start with nb1

[Install nb1 and open its local workbench](https://b1ug.github.io/nb1-guide/getting-started).
One native executable provides the CLI, optional daemon and embedded Web interface.
The matching MCP adapter and Agent Skill are optional release downloads.

## Choose the right project

| Project | What it provides |
| --- | --- |
| [nb1](https://github.com/b1ug/nb1) | Native blink(1) CLI, daemon, HTTP API, device ownership and local storage. |
| [nb1 Guide](https://github.com/b1ug/nb1-guide) · [website](https://b1ug.github.io/nb1-guide/) | English/Chinese installation guides, API reference and Agent examples. Static; no USB access. |
| [nb1 Debugger](https://github.com/b1ug/nb1-debugger) | Frontend source compiled into nb1. Uses the local daemon's HTTP API at `/demo/`. |
| [nb1 WebHID](https://github.com/b1ug/nb1-webhid) | Independent WebHID development preview and experimental Chrome reminder extension. Owns USB directly. |
| [blink(1) Models](https://github.com/b1ug/blink1-models) | Versioned MK2 enclosure geometry, assembly and attribution for the debugger, browser app and guides. |
| [Homebrew tap](https://github.com/b1ug/homebrew-tap) | Source installation for macOS and Linux, with explicit `nb1 service` management. |
| [blink1-go](https://github.com/b1ug/blink1-go) | Go SDK for blink(1) device commands, parsing and capabilities. |
| [GID](https://github.com/b1ug/gid) | Go USB HID access for native applications. |
| [colorkit](https://github.com/b1ug/colorkit) | Reusable pure-Go color types, CSS names, Hex and HSV conversions. |

The embedded workbench and Browser Tools are separate interfaces. Stop or
Disconnect the current controller before another one opens the same lamp.
Browser tools do not install a native daemon; the documentation site controls
no device. Check each repository's release and support notes before installation.

Go modules supply native Go code. The embedded frontend is maintained separately
and imported as a source-pinned, hash-verified static bundle; normal nb1 builds
need neither Node nor a recursive submodule checkout.

## Contribute

Use the relevant repository for bugs, documentation or proposed improvements.
Stable releases, development previews and planned APIs are labeled separately.
Hardware support is reported with its actual model, OS and test scope; screen
previews and cached RGB are not optical measurements.
