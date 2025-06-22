---
title: CSharp - 變數與型別
tags: [CSharp, 基礎語法, 變數, 型別]
aliases: [變數, 資料型別, 基本型別]
created: 2025-06-22
updated: 2025-06-22
status: 完成
summary: C# 中變數用來儲存資料，型別定義資料的形式與記憶體結構，包含 int、float、string 等基本型別。
---
## 📌 定義

>在 C# 中，**變數**用來儲存資料，而**資料型別**則定義這些資料的形式與記憶體大小。

---
## 🧠 常見資料型別

| 類型        | 說明     | 範例值          |
| --------- | ------ | ------------ |
| `int`     | 整數     | 1, -42, 2025 |
| `float`   | 單精度浮點數 | 3.14f        |
| `double`  | 雙精度浮點數 | 3.14159      |
| `decimal` | 高精度小數  | 99.99m       |
| `char`    | 字元     | 'A', '9'     |
| `string`  | 字串     | "Hello"      |
| `bool`    | 布林值    | true, false  |
| `var`     | 自動推斷型別 | var x = 100; |

---
## 🧪 宣告與初始化

```csharp
int age = 25;
string name = "John";
bool isActive = true;
float pi = 3.14f;
decimal money = 99.99m;
```

---
## 🔁 多變數宣告

```csharp
int x = 1, y = 2, z = 3;
```

---
## ⚠️ 注意事項

- 所有變數在使用前都**必須初始化**。
- `var` 只能在**區域變數**中使用，且**必須立即賦值**。
- C# 是**強型別語言**，型別錯誤會在編譯時報錯。

---
## 🔄 類型轉換（Casting）

```csharp
int i = 100;
double d = i;        // 隱性轉換

double pi = 3.14;
int x = (int)pi;     // 顯性轉換（會截斷小數）
```

---
### 🔒 常數（Constants）

#### 📌 定義

>常數是**不可改變的變數**，在程式執行期間其值是固定的。

---

### 🔠 `const` 常數

- **編譯期常數**：必須在宣告時立即指定值。
- 預設為 `static`，不能用 `static` 修飾。
- 適合用來定義「永遠不會變的資料」，如稅率、圓周率等。

```csharp
const double PI = 3.14159;
const int MAX_COUNT = 100;
```

---
### 🧊 `readonly` 唯讀欄位

- **執行期常數**：可在建構子中指定初始值。
    
- 只能宣告在類別層級，不能是區域變數。
    
- 適合根據環境、傳入參數來決定值，但在物件建立後就不可再變更。
    

```csharp
class MyClass
{
    public readonly int ID;

    public MyClass(int id)
    {
        ID = id; // 只能在建構子中設定一次
    }
}
```

---
### ⚖️ 比較表

|特性|`const`|`readonly`|
|---|---|---|
|指派時間|編譯時|執行時（建構子）|
|可否修改|不可|建構時可、之後不可|
|使用範圍|任何類別或區域內|僅限欄位（field）|
|支援的型別|原始型別與字串|任意型別|
|是否 static|隱含 static|需自行加上 static（可選）|
