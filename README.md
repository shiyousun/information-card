# 📊 Information Card - 智能信息可视化卡片生成器

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python 3.6+](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://www.python.org/downloads/)

> 根据关键词自动搜索概念、总结并生成 Excalidraw 手绘风格的 SVG 信息卡片。支持多关键词批量生成。

## ✨ 特色

- 🔍 **自动搜索**：输入关键词，AI 自动搜索并总结为 5-7 个要点
- 🎨 **手绘风格**：Excalidraw 风格，温暖柔和的视觉设计
- 📊 **可视化图表**：自动选择柱状图/饼图/流程图/关系图
- 🇨🇳 **中文完美**：直接写中文，内置 Unicode 安全校验
- ⚡ **批量生成**：多关键词用 `;` 分隔，一次生成多张

## 🎨 设计规范

- **尺寸**：600×800px（3:4 黄金比例）
- **风格**：Excalidraw 手绘感 + 圆角卡片
- **配色**：暖白底 + 主题色系（科技蓝/自然绿/活力橙/创意紫/温暖红）
- **字体**：KingHwa_OldSong / LXGW WenKai / Comic Sans MS

## 🚀 快速开始

### 作为 AI Skill 使用

1. 将本目录放入 `~/.claude/skills/information-card/`（或对应 IDE 的 skills 目录）
2. 在 AI 对话中输入：`/information-card 量子计算` 即可生成卡片
3. 批量生成：`/information-card 量子计算;区块链;AI Agent`

### 布局结构

```
+==========================================+
|     📌 主标题区 (关键词 + 副标题)        |
+------------------------------------------+
|     📋 清单要点区 (5-7 个 emoji+要点)    |
+------------------------------------------+
|     📊 可视化图表区 (图表/流程图)        |
+------------------------------------------+
|     底部署名 "友哥信息卡"                |
+==========================================+
```

## 📁 项目结构

```
information-card/
├── SKILL.md              # AI Skill 定义（完整 prompt + 布局规范）
├── README.md             # 本文件
└── LICENSE               # MIT License
```

## 🔧 技术要点

- **防重叠布局**：固定区域分配策略，每个区域有明确 Y 坐标范围
- **中文安全**：五条铁律防止 AI 手写 Unicode 码点出错
- **四种图表**：柱状图、饼图、流程图、关系图，根据主题自动选择
- **输出格式**：SVG（可直接在浏览器渲染）

## 📄 License

MIT License - 自由使用，欢迎 Star ⭐

## 👨‍💻 作者

**友哥** · 友哥 & AI 创造
