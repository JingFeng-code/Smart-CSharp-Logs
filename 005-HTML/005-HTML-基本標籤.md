---
title: "HTML 基本標籤"
tags: [HTML, 基礎, 標籤]
aliases: [HTML標籤, HTML基礎]
created: 2025-06-22
updated: 2025-06-22
status: "完成"
summary: "介紹 HTML 常用的基本標籤及其用途。"
---

# 005-HTML-基本標籤

---

## HTML 是什麼？

- 超文字標記語言（HyperText Markup Language）
- 用於建立網頁結構和內容的標準語言

---

## 常用基本標籤

| 標籤      | 說明                       | 範例                              |
|-----------|----------------------------|----------------------------------|
| `<html>`  | HTML 文件的根元素           | `<html> ... </html>`              |
| `<head>`  | 定義文件頭部，包含標題、元資料等 | `<head> ... </head>`              |
| `<title>` | 定義網頁標題               | `<title>我的網頁</title>`         |
| `<body>`  | 定義網頁的主要內容         | `<body> ... </body>`              |
| `<h1>`~`<h6>` | 標題標籤，數字越小標題越大 | `<h1>主標題</h1>`                 |
| `<p>`    | 段落標籤                   | `<p>這是一段文字。</p>`            |
| `<a>`    | 超連結標籤                 | `<a href="https://example.com">連結文字</a>` |
| `<img>`  | 插入圖片                   | `<img src="image.jpg" alt="描述文字" />` |
| `<ul>` / `<ol>` | 無序列表 / 有序列表       | `<ul><li>項目1</li></ul>`          |
| `<div>`  | 區塊容器                   | `<div>內容</div>`                 |
| `<span>` | 行內元素容器               | `<span>文字</span>`               |

---

## HTML 文件範例

```html
<!DOCTYPE html>
<html>
<head>
    <title>範例網頁</title>
</head>
<body>
    <h1>歡迎來到我的網站</h1>
    <p>這是一個段落文字。</p>
    <a href="https://www.example.com">前往 Example</a>
</body>
</html>
