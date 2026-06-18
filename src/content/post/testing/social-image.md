---
title: "自定义分享图示例"
publishDate: "27 January 2023"
description: "这篇文章演示如何在 frontmatter 中配置自定义社交分享图。"
tags: ["示例", "博客", "图片"]
ogImage: "/social-card.png"
---

## 给文章添加分享图

在文章 frontmatter 里添加 `ogImage` 后，这篇文章会使用指定图片作为 Open Graph 分享图，而不是自动生成图片。

```yaml
ogImage: "/social-card.png"
```

图片可以放在 `public` 目录，也可以换成你自己的公开图片地址。
