---
tags: [CSharp, OOP, 物件導向]
aliases: [物件導向概念, OOP概念]
---
## 設計物件的黃金規則

- 物件愈簡單愈好
- 物件的責任愈明確愈好
- Function中不能寫死的資料要變成參數

---

- **過程導向程式設計 (Process-Oriented Programming)**  
  強調如何一步步完成任務。

- **物件導向程式設計 (Object-Oriented Programming)**  
  強調如何設計一個能完成任務的程式。

- **類別 (Class)**  
  程式設計圖，定義程式的方法和屬性。  
  → 可以想像成「圖紙」。

- **實例 (Instance)**  
  類別的實例，是實際能執行操作的實體。  
  → 就是根據圖紙製造出來的產物。

- **方法 (Function / Method)**  
  定義類別裡面的函數，決定程式的行為。  
  → 就是產物的功能。

- **屬性 (Attributes)**  
  程式的特徵或狀態。  
  → 如產物的顏色、尺寸等規格參數。

- **繼承 (Inheritance)**  
  允許一個類別繼承另一個類別的方法與屬性。  
  → 類似產物的圖紙繼承了其他圖紙的設計（像電路圖紙）。

---

## 範例程式碼

```csharp
// 定義類別
class Animal {
    public string Name;
    public void Speak() {
        Console.WriteLine("Animal speaks");
    }
}

// 建立實例
Animal dog = new Animal();
dog.Name = "Dog";
dog.Speak(); // 輸出：Animal speaks
