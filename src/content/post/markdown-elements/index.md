---
title: "Markdown 元素示例"
description: "这篇文章用于测试和展示常见 Markdown 元素。"
publishDate: "22 Feb 2023"
updatedDate: 22 Jan 2024
tags: ["测试", "markdown"]
pinned: true
---

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题

## 分割线

---

## 强调

**这是粗体**

_这是斜体_

~~这是删除线~~

## 引用

> 这是一段引用。
>
> > 引用也可以嵌套。

## 脚注

这里有一个脚注引用[^1]。

[^1]: 这是脚注内容。

## 列表

无序列表：

- 第一项
- 第二项
  - 子项目
- 第三项

有序列表：

1. 第一步
2. 第二步
3. 第三步

## 代码

行内代码：`const site = "my-site"`

代码块：

```js title="demo.js"
function add(a, b) {
	return a + b;
}

console.log(add(2, 3));
```

## 表格

| 项目 | 说明 |
| --- | --- |
| posts | 文章内容 |
| tags | 标签页面 |

## 图片

同目录图片：`src/content/post/markdown-elements/logo.png`

![Astro Cactus 标志](./logo.png)

## 链接

[Astro 文档](https://docs.astro.build/)
