---
title: "HTML 基本標籤"
tags: [HTML, 基礎, 標籤]
aliases: [HTML標籤, HTML基礎]
created: 2025-06-22
updated: 2025-06-22
status: "完成"
summary: "介紹 HTML 常用的基本標籤及其用途。"
---
---
## HTML 是什麼？

- 超文字標記語言（HyperText Markup Language）
- 用於建立網頁結構和內容的標準語言

---
## 常用基本標籤

| 標籤       | 說明                         | 範例                              |
|------------|------------------------------|----------------------------------|
| `<html>`   | HTML 文件的根元素             | `<html> ... </html>`              |
| `<head>`   | 定義文件頭部，包含標題、元資料等 | `<head> ... </head>`              |
| `<title>`  | 定義網頁標題                 | `<title>我的網頁</title>`         |
| `<body>`   | 定義網頁的主要內容           | `<body> ... </body>`              |
| `<h1>`~`<h6>` | 標題標籤，數字越小標題越大 | `<h1>主標題</h1>`                 |
| `<p>`      | 段落標籤                     | `<p>這是一段文字。</p>`            |
| `<a>`      | 超連結標籤                   | `<a href="https://example.com">連結文字</a>` |
| `<img>`    | 插入圖片                     | `<img src="image.jpg" alt="描述文字" />` |
| `<ul>`     | 無序列表                     | `<ul><li>項目1</li></ul>`          |
| `<ol>`     | 有序列表                     | `<ol><li>項目1</li></ol>`          |
| `<li>`     | 列表項目                     | `<li>清單項目</li>`               |
| `<div>`    | 區塊容器                     | `<div>內容</div>`                 |
| `<span>`   | 行內元素容器                 | `<span>文字</span>`               |
| `<table>`  | 表格容器                    | `<table>...</table>`              |
| `<tr>`     | 表格列                      | `<tr>...</tr>`                   |
| `<td>`     | 表格欄位（儲存格）           | `<td>內容</td>`                  |
| `<th>`     | 表格標頭                    | `<th>標題</th>`                  |

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
```

## HTML表格範例

```html
<table border="1">
  <tr>
    <th>姓名</th>
    <th>年齡</th>
  </tr>
  <tr>
    <td>小明</td>
    <td>18</td>
  </tr>
  <tr>
    <td>小華</td>
    <td>20</td>
  </tr>
</table>
```