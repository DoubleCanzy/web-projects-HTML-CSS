
#还可以做CSS优化

# single-page-cv · 单页简历

- **类型**：小文档（纯 HTML 单页）
- **参考**：[roadmap.sh — Single-Page CV](https://roadmap.sh/projects/single-page-cv)

## 文件结构

| 文件 | 说明 |
| ---- | ---- |
| `index.html` | 简历页面本体（纯 HTML，无样式） |
| `favicon.svg` | 网站图标（SVG 格式） |
| `README.md` | 本文档 |

## 需求对照

| 参考项目要求 | 实现位置 |
| ------------ | -------- |
| 语义化 HTML 结构 | `header` / `address` / `main` / `section` / `article` / `footer` / `nav` |
| 单页布局（技能、教育、工作经历） | `main` 内三个 `section` |
| SEO meta 标签 | `head` 中 `description` / `keywords` / `author` / `robots` / `canonical` |
| Open Graph 标签 | `og:type` / `og:title` / `og:description` / `og:url` / `og:image` / `og:locale` |
| favicon | `<link rel="icon">` 指向 `favicon.svg` |

## 语义标签小讲解

- `<header>`：页眉，放姓名、职位、联系方式等个人概要
- `<address>`：专门用于标记联系信息（地址、电话、邮箱）
- `<main>`：页面唯一主体内容区
- `<section>` + 内部标题：划分「技能 / 教育 / 工作经历」各大区块
- `<article>`：可独立成篇的条目（一条教育经历、一段工作经历）
- `<footer>` + `<nav>`：页脚与外部链接导航

## 使用说明

- 双击 `index.html` 即可在浏览器中打开预览
- 简历内容为虚构示例，替换成你自己的信息即可
- 上线前需要替换：`canonical` 与 `og:url` 的地址；`og-image.png` 是自动生成的占位封面图（1200×630，蓝底白字），正式使用请换成你自己的图
- roadmap 建议本项目**暂不加 CSS**——语义结构先行，样式留给后续项目（Basic HTML Website）处理
