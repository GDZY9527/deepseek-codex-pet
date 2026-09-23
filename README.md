# DeepSeek Pet for Codex

[English](README.md) | [中文](README.zh-CN.md)

A Codex/Hatch Pet v2 package based on the supplied DeepSeek blue chibi character artwork.

![DeepSeek animation spritesheet](spritesheet.png)

## Overview

This is a DeepSeek animated pet package for the built-in Codex pet system, not a standalone desktop application. It follows the Hatch Pet v2 atlas contract while preserving the character's original clothing, hairstyle, colors, and overall identity.

## Installation

Download or clone this repository, then copy the entire repository directory to:

```text
%CODEX_HOME%\pets\deepseek
```

When `CODEX_HOME` is not explicitly configured on Windows, the usual location is:

```text
%USERPROFILE%\.codex\pets\deepseek
```

The final installation should contain at least:

```text
%USERPROFILE%\.codex\pets\deepseek\
├── pet.json
└── spritesheet.png
```

Restart Codex, open **Settings → Pets**, and select **DeepSeek**.

## Package contents

- `pet.json` — Codex custom-pet manifest.
- `spritesheet.png` — production RGBA animation atlas.
- `preview.png` — labeled animation contact sheet.
- `validation.json` — deterministic Hatch Pet atlas validation result.
- `checksums.sha256` — SHA-256 checksums for the distributable assets.

## Atlas contract

- `spriteVersionNumber`: 2
- Dimensions: 1536 × 2288 px
- Grid: 8 columns × 11 rows
- Cell size: 192 × 208 px
- Standard animation rows: 9
- Clockwise look directions: 16
- Transparent RGB residue: 0 pixels

## Animation notes

The jump row preserves the first five authored poses so Codex's longer final-frame hold lands on the airborne star pose, retaining the original clear and slightly snappy jump rhythm.
