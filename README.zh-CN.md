# DeepSeek Codex 桌面宠物

[English](README.md) | [中文](README.zh-CN.md)

基于 DeepSeek 蓝色 Q 版角色素材制作的 Codex / Hatch Pet v2 内置桌面宠物。

![DeepSeek 动画图集](spritesheet.png)

## 简介

这是一个适用于 Codex 内置宠物系统的 DeepSeek 动画宠物包，不是独立运行的桌面程序。宠物使用 Hatch Pet v2 图集规范，并保留了角色原有的服装、发型、配色与整体形象。

## 安装方法

下载或克隆本仓库，然后将整个仓库目录复制到：

```text
%CODEX_HOME%\pets\deepseek
```

如果 Windows 中没有单独配置 `CODEX_HOME`，通常使用：

```text
%USERPROFILE%\.codex\pets\deepseek
```

安装目录至少应包含：

```text
%USERPROFILE%\.codex\pets\deepseek\
├── pet.json
└── spritesheet.png
```

复制完成后重启 Codex，然后进入 **设置 → 宠物**，选择 **DeepSeek**。

## 包含文件

- `pet.json` — Codex 自定义宠物清单。
- `spritesheet.png` — 实际使用的 RGBA 动画图集。
- `preview.png` — 带动作标签的动画预览图。
- `validation.json` — Hatch Pet 图集自动验证结果。
- `checksums.sha256` — 发布资源的 SHA-256 校验值。

## 图集规格

- `spriteVersionNumber`：2
- 图集尺寸：1536 × 2288 px
- 网格：8 列 × 11 行
- 单帧尺寸：192 × 208 px
- 标准动画：9 行
- 顺时针观察方向：16 个
- 透明像素 RGB 残留：0

## 动画说明

跳跃动作保留了原始前五帧，使 Codex 对末帧的较长停留落在带星光的腾空姿势上，从而保留原动画清晰、轻微顿挫的起跳节奏。
