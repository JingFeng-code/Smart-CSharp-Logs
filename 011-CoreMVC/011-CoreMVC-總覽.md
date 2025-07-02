---
title: 🧩 ASP.NET Core MVC 總覽
tags:
  - ASP.NET Core
  - MVC
  - CSharp
  - 網頁後端
  - 架構設計
aliases:
  - CoreMVC
  - ASP.NET Core MVC
  - MVC 架構
created: 2025-07-02
updated: 2025-07-02
status: 草稿
summary: 本筆記系統化彙整 ASP.NET Core MVC 的核心架構、開發流程與現代實務，包括 Controller、View、Model、Routing、驗證、Razor、依賴注入、資料庫、分層設計、安全性、效能、測試與部署，適合作為後端開發快速查閱與整合參考。
---

## 📘 Core MVC 筆記索引

- [[011.1-CoreMVC-框架介紹與專案結構]]
- [[011.2-CoreMVC-路由與控制器 (Controller)]]
- [[011.3-CoreMVC-模型設計與資料綁定 (Model)]]
- [[011.4-CoreMVC-視圖與 Razor 語法 (View)]]
- [[011.5-CoreMVC-表單處理與驗證]]
- [[011.6-CoreMVC-依賴注入與服務註冊]]
- [[011.7-CoreMVC-與資料庫整合 (EF Core)]]
- [[011.8-CoreMVC-分層架構與專案實務設計]]
- [[011.9-CoreMVC-錯誤處理與中介軟體 (Middleware)]]
- [[011.10-CoreMVC-安全性與授權 (Authentication & Authorization)]]
- [[011.11-CoreMVC-效能優化與快取]]
- [[011.12-CoreMVC-單元測試與自動化]]
- [[011.13-CoreMVC-部署與維運]]

---

## 🏷️ 主題簡介

- **框架介紹與專案結構**：ASP.NET Core MVC 架構原理、專案目錄與檔案組成。
- **路由與控制器**：URL 路由機制、Controller 設計與 Action 方法。
- **模型設計與資料綁定**：Model 類別、ViewModel、資料驗證與自動綁定。
- **視圖與 Razor 語法**：View 檔案、Razor 標記語法、版型與部分檢視。
- **表單處理與驗證**：表單送出流程、伺服器端/用戶端驗證、ModelState。
- **依賴注入與服務註冊**：DI 容器、Service Lifetime、註冊與解析服務。
- **與資料庫整合（EF Core）**：ORM 基本操作、DbContext、Migrations、LINQ 查詢。
- **分層架構與專案實務設計**：Repository、Service Layer、專案模組化。
- **錯誤處理與中介軟體**：例外處理、全域錯誤攔截、自訂 Middleware。
- **安全性與授權**：身分驗證（Identity）、授權（Role/Policy）、防範 CSRF/XSS。
- **效能優化與快取**：Response Caching、資料快取、非同步程式設計、資源壓縮。
- **單元測試與自動化**：Controller/Service 單元測試、Mock 依賴、自動化測試流程。
- **部署與維運**：雲端部署（Azure）、CI/CD、組態管理、日誌監控。

---

## 🔁 延伸閱讀

- [[001-CSharp-基礎語法總覽]]
- [[004-ADO.NET總覽]]
- [[007-LINQ-總覽]]
- [[008-JS-總覽]]
- [[XXX-WebAPI-總覽]]（Web API 模組，適合前後端分離需求）

---

## 🏆 筆記設計說明

- 本結構兼顧**基礎教學**與**企業實務**，涵蓋現代 ASP.NET Core MVC 專案常見需求與最佳實踐。
- 可依需求擴充各主題細節，並搭配實作範例、錯誤排查與效能優化建議，提升查閱與應用效率。
