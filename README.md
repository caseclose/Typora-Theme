# Typora Academic Theme

基于 [Typora 官方 Academic 主题](https://theme.typora.io/theme/Academic/) 的个性化修改版，更适合中文写作与 PDF 导出。

A customized fork of the official Typora Academic theme, tuned for Chinese typography and PDF export.

## 特性 / Features

- 正文使用 Times New Roman + 华文楷体（STKaiti），兼顾中英文阅读体验
- 等宽字体使用 Latin Modern Mono Light，代码块风格接近 LaTeX
- 标题居中、正文两端对齐，整体排版偏学术论文风格
- 加粗文字显示为红色，便于强调重点
- 针对 PDF 导出优化了页边距（`@page` 规则）

## 目录结构 / Structure

```
Typora-Theme/
├── academic.css          # 主题样式文件
└── academic/             # 字体与许可文件
    ├── *.woff
    ├── GUST e-foundry License.txt
    └── STIX_2.0.0_license.pdf
```

安装时需将 `academic.css` 与 `academic/` 文件夹**一并**复制到 Typora 主题目录，保持相对路径不变。

## 安装 / Installation

1. 下载本仓库（Clone 或 Download ZIP）
2. 在 Typora 中打开主题文件夹：**偏好设置 → 外观 → 打开主题文件夹**
3. 将 `academic.css` 和 `academic/` 文件夹复制到该目录
4. 重启 Typora，在菜单 **主题 → Academic** 中选择

### 各平台主题目录

| 平台 | 路径 |
|------|------|
| macOS | `~/Library/Application Support/abnerworks.Typora/themes/` |
| Windows | `%APPDATA%\Typora\themes\` |
| Linux | `~/.config/Typora/themes/` |

## 与官方主题的差异 / Changes from Official

| 项目 | 官方 Academic | 本主题 |
|------|---------------|--------|
| 正文字体 | STIX2Text | Times New Roman, STKaiti |
| 编辑区内边距 | 10% / 5% | 5% / 2.5% |
| PDF 页边距 | 默认 | 上下 1cm，左右 0.25cm |
| 加粗样式 | 默认黑色 | 红色 |

如需进一步自定义，可在主题目录下创建 `academic.user.css`，仅对本主题生效，且不会被主题更新覆盖。

## 字体许可 / Font Licenses

- **STIX 字体**：见 `academic/STIX_2.0.0_license.pdf`
- **Latin Modern Mono**：见 `academic/GUST e-foundry License.txt`

## 致谢 / Credits

- 原始主题：[Typora Academic Theme](https://theme.typora.io/theme/Academic/)
- 字体来源：STIX Fonts Project、GUST e-foundry
