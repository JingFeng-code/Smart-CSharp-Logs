---
title: 🧩 ASP.NET Core MVC 總覽
tags:
  - ASP-NET
  - Core
  - MVC
  - CSharp
  - 網頁後端
  - 架構設計
aliases:
  - CoreMVC
  - ASP.NET Core MVC
  - MVC 架構
created: 2025-07-05
updated: 2025-07-05
status: 草稿
summary: 本筆記系統化彙整 ASP.NET Core MVC 的核心架構、開發流程與現代實務，包括 Controller、View、Model、Routing、驗證、Razor、依賴注入、資料庫、分層設計、安全性、效能、測試與部署，並新增非同步、組態管理、日誌記錄與Web API整合等重要主題，適合作為後端開發快速查閱與整合參考。
---

## 📘 Core MVC 筆記索引

- [[011.1-CoreMVC-框架介紹與專案結構]]
- [[011.2-CoreMVC-路由與控制器 (Controller)]]
- [[011.3-CoreMVC-模型設計與資料綁定 (Model)]]
- [[011.4-CoreMVC-視圖與 Razor 語法 (View)]]
- [[011.5-CoreMVC-表單處理與驗證]]
- [[011.6-CoreMVC-依賴注入與服務註冊]]
- [[011.7-CoreMVC-與資料庫整合 (EF Core)]]
- [[011.8-CoreMVC-非同步程式設計 (Async Await)]]
- [[011.9-CoreMVC-組態管理與環境設定 (Configuration)]]
- [[011.10-CoreMVC-日誌記錄與監控 (Logging)]]
- [[011.11-CoreMVC-錯誤處理與中介軟體 (Middleware)]]
- [[011.12-CoreMVC-安全性與授權 (Authentication & Authorization)]]
- [[011.13-CoreMVC-效能優化與快取]]
- [[011.14-CoreMVC-單元測試與自動化]]
- [[011.15-CoreMVC-部署與維運]]
- [[011.16-CoreMVC-MVC與WebAPI整合考量]]

---

## 🏷️ 主題簡介

- **框架介紹與專案結構**：ASP.NET Core MVC 架構原理、專案目錄與檔案組成。

- **路由與控制器**：URL 路由機制、Controller 設計與 Action 方法。

- **模型設計與資料綁定**：Model 類別、ViewModel、資料驗證與自動綁定。

- **視圖與 Razor 語法**：View 檔案、Razor 標記語法、版型與部分檢視、**Tag Helpers 與 View Components 應用**。

- **表單處理與驗證**：表單送出流程、伺服器端/用戶端驗證、ModelState、**Ajax 表單處理**。

- **依賴注入與服務註冊**：DI 容器、Service Lifetime、註冊與解析服務。

- **與資料庫整合（EF Core）**：ORM 基本操作、DbContext、Migrations、LINQ 查詢。

- **非同步程式設計 (Async Await)**：`async`/`await` 原理與應用、非同步陷阱與最佳實踐。

- **組態管理與環境設定 (Configuration)**：`appsettings.json`、多環境配置、環境變數、機敏資料保護。

- **日誌記錄與監控 (Logging)**：ASP.NET Core 內建 Logging、常用日誌框架（如 Serilog）、日誌等級與策略。

- **錯誤處理與中介軟體**：例外處理、全域錯誤攔截、自訂 Middleware。

- **安全性與授權**：身分驗證（Identity）、授權（Role/Policy）、防範 CSRF/XSS。

- **效能優化與快取**：Response Caching、資料快取、資源壓縮。

- **單元測試與自動化**：Controller/Service 單元測試、Mock 依賴、自動化測試流程。

- **部署與維運**：雲端部署（Azure）、CI/CD、應用程式監控。

- **MVC 與 WebAPI 整合考量**：MVC 與 RESTful API 設計差異、共用邏輯與資料格式處理、**API 版本控制**。

---

## 🔁 延伸閱讀

- [[001-CSharp-基礎語法總覽]]
- [[004-ADO.NET總覽]]
- [[007-LINQ-總覽]]
- [[008-JS-總覽]]
- [[XXX-WebAPI-總覽]]

---

## 🏆 筆記設計說明

- 本結構兼顧**基礎教學**與**企業實務**，涵蓋現代 ASP.NET Core MVC 專案常見需求與最佳實踐。
- 新增了 **「非同步程式設計」、「組態管理」、「日誌記錄」** 等在現代應用開發中極為重要的主題。
- 強化了**「視圖」和「表單處理」**部分，使其能更好地銜接前端整合。
- 獨立出 **「MVC 與 WebAPI 整合考量」**，幫助理解兩種模式的共存與選擇。
- 可依需求擴充各主題細節，並搭配實作範例、錯誤排查與效能優化建議，提升查閱與應用效率。