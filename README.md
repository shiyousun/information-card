# 📊 Information Card - 智能信息可视化卡片生成器 | Smart Info Visualization Card Generator

<p align="center">
  <img src="https://img.shields.io/badge/SVG-Excalidraw%20Style-orange.svg" alt="SVG">
  <img src="https://img.shields.io/badge/AI-Skill-green.svg" alt="AI Skill">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License">
</p>

<p align="center"><b>📖 <a href="#中文">中文</a> | <a href="#english">English</a></b></p>

---

<a name="中文"></a>

## 🇨🇳 中文

> **输入关键词，AI 自动搜索概念、总结为 5-7 个要点，并生成 Excalidraw 手绘风格的 SVG 信息卡片。** 支持多关键词批量生成，中文完美呈现。

### ✨ 核心功能

- 🔍 **自动搜索**：输入关键词，AI 自动搜索互联网并总结为 5-7 个核心要点
- 🎨 **手绘风格**：Excalidraw 手绘感设计，温暖柔和的视觉体验
- 📊 **可视化图表**：自动选择最适合的图表类型（柱状图 / 饼图 / 流程图 / 关系图）
- 🇨🇳 **中文完美**：直接写中文字符，内置 Unicode 安全校验（五条铁律防止码点错误）
- ⚡ **批量生成**：多关键词用 `;` 分隔，一次生成多张卡片
- 🎨 **五色主题**：科技蓝 / 自然绿 / 活力橙 / 创意紫 / 温暖红，根据主题自动匹配

### 🎨 设计规范

| 属性 | 规格 |
|------|------|
| **尺寸** | 600×800px（3:4 黄金比例） |
| **风格** | Excalidraw 手绘感 + 圆角卡片 |
| **配色** | 暖白底 (#FEFEFE) + 主题色系 |
| **字体** | KingHwa_OldSong / LXGW WenKai / Comic Sans MS |
| **布局** | 标题区 → 清单要点区 → 可视化图表区 → 底部署名 |

### 🚀 使用方式

#### 作为 AI Skill

1. 将本目录放入 `~/.claude/skills/information-card/`
2. 在 AI 对话中输入：`/information-card 量子计算`
3. 批量生成：`/information-card 量子计算;区块链;AI Agent`

#### 布局结构

```
+==========================================+
|     📌 主标题区 (关键词 + 副标题)         |
+------------------------------------------+
|     📋 清单要点区 (5-7 个 emoji + 要点)   |
+------------------------------------------+
|     📊 可视化图表区 (图表/流程图)          |
+------------------------------------------+
|     底部署名 "友哥信息卡"                  |
+==========================================+
```

### 📁 项目结构

```
information-card/
├── SKILL.md      # AI Skill 定义（完整 prompt + 布局规范 + 五条铁律）
├── README.md     # 本文件
└── LICENSE       # MIT License
```

### 🔧 技术要点

- **防重叠布局**：固定区域分配策略，每个区域有明确 Y 坐标范围
- **中文安全五条铁律**：防止 AI 手写 Unicode 码点出错
- **四种图表自动选择**：柱状图（数值对比）、饼图（占比分布）、流程图（步骤过程）、关系图（概念关联）
- **输出格式**：标准 SVG，可直接在浏览器渲染

---

<a name="english"></a>

## 🇬🇧 English

> **Enter a keyword, and AI automatically searches the concept, summarizes it into 5-7 key points, and generates an Excalidraw-style hand-drawn SVG information card.** Supports batch generation with multiple keywords.

### ✨ Key Features

- 🔍 **Auto Search**: Input a keyword, AI searches the web and summarizes into 5-7 core points
- 🎨 **Hand-Drawn Style**: Excalidraw-inspired design with warm, soft visual aesthetics
- 📊 **Auto Chart Selection**: Automatically chooses the best chart type (bar / pie / flow / relation)
- 🇨🇳 **Perfect Chinese**: Direct Chinese character rendering with built-in Unicode safety checks
- ⚡ **Batch Generation**: Separate multiple keywords with `;` to generate multiple cards at once
- 🎨 **Five Color Themes**: Tech Blue / Nature Green / Vibrant Orange / Creative Purple / Warm Red, auto-matched by topic

### 🎨 Design Specifications

| Property | Specification |
|----------|--------------|
| **Size** | 600×800px (3:4 golden ratio) |
| **Style** | Excalidraw hand-drawn feel + rounded cards |
| **Colors** | Warm white base (#FEFEFE) + theme color palette |
| **Fonts** | KingHwa_OldSong / LXGW WenKai / Comic Sans MS |
| **Layout** | Title → Key Points List → Visualization Chart → Footer |

### 🚀 Usage

#### As AI Skill

1. Place this directory in `~/.claude/skills/information-card/`
2. In AI conversation: `/information-card quantum computing`
3. Batch: `/information-card quantum computing;blockchain;AI Agent`

#### Layout Structure

```
+==========================================+
|     📌 Title Area (keyword + subtitle)    |
+------------------------------------------+
|     📋 Key Points (5-7 emoji + points)    |
+------------------------------------------+
|     📊 Visualization (chart/flowchart)    |
+------------------------------------------+
|     Footer "YooGe Info Card"              |
+==========================================+
```

### 📁 Project Structure

```
information-card/
├── SKILL.md      # AI Skill definition (full prompt + layout spec + safety rules)
├── README.md     # This file
└── LICENSE       # MIT License
```

### 🔧 Technical Details

- **Anti-Overlap Layout**: Fixed zone allocation with explicit Y-coordinate ranges for each section
- **Chinese Safety (5 Rules)**: Prevents AI from incorrectly hand-writing Unicode code points
- **4 Auto-Selected Chart Types**: Bar chart (numeric comparison), Pie chart (distribution), Flowchart (process steps), Relation graph (concept connections)
- **Output Format**: Standard SVG, directly renderable in browsers

---

## 📄 License

MIT License - 自由使用 | Free to use

## 👨‍💻 Author / 作者

**友哥 (YooGe)** · 友哥 & AI 创造 | Created by YooGe & AI
