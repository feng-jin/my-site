---
title: "Markdown 提示块"
description: "这篇文章展示 Astro Cactus 中的 Markdown 提示块功能。"
publishDate: "25 Aug 2024"
updatedDate: "4 July 2025"
tags: ["markdown", "提示块"]
---

## 提示块是什么

提示块适合放补充信息、注意事项或警告内容。

## 怎么使用

用三个冒号包住 Markdown 内容，并在开头写提示块类型：

```md
:::note
这是一条普通提示。
:::
```

渲染效果：

:::note
这是一条普通提示。
:::

## 支持的类型

- `note`
- `tip`
- `important`
- `warning`
- `caution`

### Note

:::note
普通提示，适合放补充说明。
:::

### Tip

:::tip
小技巧，适合放更顺手的做法。
:::

### Important

:::important
重要信息，适合放必须注意的内容。
:::

### Caution

:::caution
谨慎操作，可能会产生负面影响。
:::

### Warning

:::warning
警告内容，适合放高风险提醒。
:::

## 自定义标题

```md
:::note[自定义标题]
这是一条带自定义标题的提示。
:::
```

效果：

:::note[自定义标题]
这是一条带自定义标题的提示。
:::

## GitHub 仓库卡片

可以用指令插入 GitHub 仓库卡片：

::github{repo="chrismwilliams/astro-theme-cactus"}

也可以插入 GitHub 用户卡片：

::github{user="withastro"}
