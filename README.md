# Blackhole-macOS

> [!NOTE]
> 基于 [huiyeruzhou/ghostty-blackhole-macos](https://github.com/huiyeruzhou/ghostty-blackhole-macos) 修改，原项目作者 [huiyeruzhou](https://github.com/huiyeruzhou) · [XboxNahida](https://github.com/XboxNahida) · [MoMing-ink](https://github.com/MoMing-ink)

黑洞屏保 macOS 菜单栏应用。基于 Eric Bruneton 的黑洞着色器，实时渲染引力透镜效果。

## 功能
- 菜单栏图标 + 下拉菜单控制
- Always Show / Idle Detection 两种模式
- 16 个预设效果，可自定义配置
- 全屏 ScreenCaptureKit 桌面透镜

## 依赖
- macOS 12.3+
- [cmake](https://cmake.org) 3.20+
- [glfw](https://www.glfw.org) 3.4+
- Xcode Command Line Tools（`xcode-select --install`）

## 构建
```bash
brew install cmake glfw
cmake -S . -B _build/macos -DCMAKE_BUILD_TYPE=Release
cmake --build _build/macos --config Release
open _build/macos/blackhole-macos.app
```

## 使用
首次运行需在 **系统设置 → 隐私与安全性 → 屏幕录制** 中授权，方可捕捉桌面实现透镜效果。
点击菜单栏图标打开下拉菜单，选择模式、闲置时间和预设后点 Start。

## 许可证
MIT
