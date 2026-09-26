# Homebrew Tap · StandardCode

[StandardCode](https://github.com/admin001-bit/standardcode)（开源 CLI 编码代理）的 Homebrew 安装通道 —— macOS / Apple Silicon (arm64)。

## 安装

```bash
# 推荐：完全限定名安装——Homebrew 仅信任该 formula（无需额外授权步骤）
brew install admin001-bit/tap/standardcode

# 或：先信任该 formula，再按短名安装
brew tap admin001-bit/tap
brew trust --formula admin001-bit/tap/standardcode
brew install standardcode
```

> Homebrew ≥6.0.0 起，非官方 tap 默认不受信任：按**短名**安装前须先信任该 formula（或信任整个 tap）；**完全限定名**安装则自动仅信任该 formula。详见官方 [Tap Trust](https://docs.brew.sh/Tap-Trust)。

## 说明

- **仅 Apple Silicon**：上游只发布 `darwin-arm64` 单文件产物（无 Intel 产物）。
- **未签名 / 未公证**：二进制**未**做代码签名与公证，首次运行可能被 Gatekeeper 提示"来源未知"（属预期行为）；完整性以 SHA-256 为通道 —— formula 内 `sha256` 即[上游 Release](https://github.com/admin001-bit/standardcode/releases) 资产的校验值。
- formula 的 `url` / `sha256` 直接指向上游 GitHub Release 资产；本 tap 不另行分发二进制。

## 更新 / 卸载

```bash
brew update && brew upgrade standardcode
brew uninstall standardcode
```
