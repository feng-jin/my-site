---
title: "给站点添加 Webmentions"
description: "这篇文章记录如何给个人网站添加 Webmentions 互动。"
publishDate: "11 Oct 2023"
tags: ["webmentions", "astro", "社交"]
updatedDate: 6 December 2024
pinned: true
---

## 简版步骤

1. 在首页添加指向 GitHub 或邮箱的个人链接。
2. 用你的域名注册 [Webmention.io](https://webmention.io/)。
3. 在 `.env` 里配置 `WEBMENTION_URL` 和 `WEBMENTION_API_KEY`。
4. 在 [brid.gy](https://brid.gy/) 连接你想同步的社交账号。
5. 重新构建并发布站点。

## Webmentions 是什么

Webmentions 可以把其他网站或社交平台上对你文章的喜欢、评论和回复展示到文章底部。

这个模板目前展示喜欢、提及和回复。转发等其他类型先不处理，等真的需要再加。

## 配置个人链接

你需要在站点上放一个能证明身份的链接，例如 GitHub：

```html
<a href="https://github.com/your-username" rel="me">GitHub</a>
```

如果使用 `src/components/SocialList.astro`，可以给对应链接加上 `isWebmention`，组件会自动加上 `rel="me authn"`。

## 配置 Webmention.io

注册后，Webmention.io 会给你一个 feed 地址和 API key。把它们写进环境变量：

```bash
WEBMENTION_URL="你的 feed 地址"
WEBMENTION_API_KEY="你的 API key"
```

:::note
`WEBMENTION_PINGBACK` 是可选项。先不配也可以，够用再说。
:::

## 测试

发布后可以用 [webmentions.rocks](https://webmention.rocks/receive/1) 发送测试 Webmention。测试通过后，重新构建站点就能在文章底部看到互动。
