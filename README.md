# Homebrew Tap · StandardCode

[StandardCode](https://github.com/admin001-bit/standardcode)（开源 CLI 编码代理）的 Homebrew 安装通道 —— macOS / Apple Silicon (arm64)。

## 安装

```bash
brew tap admin001-bit/tap
brew install standardcode
```

> Homebrew ≥6.0.0 对非官方 tap 默认不受信任：首次安装按 brew 的交互提示授权即可（官方说明：[Tap Trust](https://docs.brew.sh/Tap-Trust)）。

## 说明

- **仅 Apple Silicon**：上游只发布 `darwin-arm64` 单文件产物（无 Intel 产物）。
- **未签名 / 未公证**：二进制**未**做代码签名与公证，首次运行可能被 Gatekeeper 提示"来源未知"（属预期行为）；完整性以 SHA-256 为通道 —— formula 内 `sha256` 即[上游 Release](https://github.com/admin001-bit/standardcode/releases) 资产的校验值。
- formula 的 `url` / `sha256` 直接指向上游 GitHub Release 资产；本 tap 不另行分发二进制。

## 更新 / 卸载

```bash
brew update && brew upgrade standardcode
brew uninstall standardcode
```
