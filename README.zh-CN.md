# Landing Craft

[![CI](https://github.com/can4hou6joeng4/landing-craft/actions/workflows/ci.yml/badge.svg)](https://github.com/can4hou6joeng4/landing-craft/actions/workflows/ci.yml)
[![GitHub release](https://img.shields.io/github/v/release/can4hou6joeng4/landing-craft)](https://github.com/can4hou6joeng4/landing-craft/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

一个 [Claude Code](https://claude.ai/claude-code) 技能，用 57 种城市风格设计系统生成**视觉大胆的落地页**。

**[在线演示](https://can4hou6joeng4.github.io/landing-craft/)** | **[更新日志](CHANGELOG.md)** | **[贡献指南](CONTRIBUTING.md)** | **[English](README.md)**

> 不是千篇一律的卡片网格模板。每一个输出都是设计作品——clip-path 分隔线、GSAP 滚动动画、SVG 纹理、真实的层次与深度。

## 它能做什么

告诉这个技能你的产品是什么。它会在浏览器中打开 **57 种城市风格的交互式预览**——从京都到拉各斯到棕榈泉——点击选择即可。然后它会生成一个包含真实产品文案的完整多文件站点。

```
你的产品-landing/
├── index.html      # 完整页面：导航、板块、页脚
├── style.css       # 设计 token、纹理、clip-path
├── main.js         # GSAP ScrollTrigger 动画
├── about.html      # 可选子页面
├── contact.html    # 可选子页面
├── blog.html       # 可选子页面
└── assets/
    └── icons.svg   # 匹配城市美学的 SVG 精灵图
```

## 核心特性

- **57 种城市美学** — 每种都有独特的字体、配色、纹理、动效和图标风格
- **交互式预览** — 浏览器端卡片选择器（非命令行菜单）
- **7 种 Hero 变体** — 全屏铺张、分屏张力、极简下降、产品演示、文字爆炸、杂志撕裂、弹出卡片
- **6 种功能布局** — 大数字、交替展示、时间线、本托格子、水平滚动、问答展开
- **6 种评价样式** — 紧凑卡片、杂志引用、马赛克拼贴、滚动横条、对话气泡、头像墙
- **4 种导航风格** — 全屏爆开、磁性胶囊、侧边垂直、拆分居中
- **3 种色调** — 城市原色、暗黑奢华、明亮现代
- **暗色模式切换** — 运行时亮暗切换，localStorage 持久化
- **多页面支持** — 可选生成关于、联系、博客子页面，共享同一设计系统
- **3 种表单板块** — 邮件订阅、等待列表、内嵌联系表单
- **6 种扩展板块** — 团队成员、数据统计、品牌滚动墙、作品集、技术集成、时间线
- **过渡风格选择** — 几何锐利 / 有机柔和 / 渐变融合 / 极简线条
- **一键部署** — 可选部署到 Netlify、Vercel 或 GitHub Pages
- **Python 3.6+ 兼容** — macOS 默认 Python 3.9 可用
- **跨平台** — Python 启动器 + Windows PowerShell 备选

## 快速开始

这是一个 Claude Code 技能。全局安装：

```bash
npx skills add can4hou6joeng4/landing-craft -a claude-code -g -y
```

然后对 Claude 说：

> "帮我做一个落地页"

## 触发词

以下词句会激活技能：`帮我做一个落地页`、`做个首页`、`产品展示页`、`活动页`、`营销页`、`官网首页`、`landing page`、`product page`、`promo page`、`make me a homepage`、`build a product showcase`、`create a campaign page`。

## 工作流程

1. **描述你的产品** — 名称 + 一句话介绍
2. **选择城市风格** — 57 张卡片在浏览器中实时渲染
3. **选择选项** — 排版、导航、色调、过渡效果、Hero/Features 变体
4. **获取站点** — 完整的 `index.html` + `style.css` + `main.js` + `icons.svg`
5. **预览** — 自动在浏览器中打开
6. **部署** — 可选一键发布到 Netlify / Vercel / GitHub Pages

## 设计哲学

- **禁止纯白背景** — 暖中性色、冷灰调或深暗色
- **至少两种字体** — 展示用衬线标题 + 干净的无衬线正文
- **SVG 作为设计核心** — 不是装饰点缀
- **GSAP 空间深度** — 视差层、粘性面板、交错揭示
- **禁止克隆网格** — 每个重复板块都有视觉层级，而非相同的行

## 许可证

[MIT](LICENSE)
