---
title: 🐳 Docker 總覽
tags:
  - Docker
  - 容器化
  - 開發環境
  - DevOps
aliases:
  - Docker Overview
  - Docker入門
  - 容器開發工具
created: 2025-07-23
updated: 2025-07-23
status: 完成
summary: 本文整理 Docker 的核心概念、基本操作流程與常用工具，並提供細部筆記索引，協助開發者理解容器化的實作與最佳實踐。
---

## Docker 是什麼？

Docker 是一個開源容器化平台，讓開發者能將應用程式與其相依環境打包成獨立容器（Container），可在任何支援 Docker 的系統上快速部署與執行。

Docker 的核心優勢在於：

- 一致性環境（解決「在我電腦上可以跑」問題）

- 快速啟動與重現

- 易於整合 DevOps / CI/CD

- 跨平台部署（本地、雲端、邊緣設備）

## 核心概念

- **Image（映像檔）**：一個唯讀的程式包，包含應用程式與其依賴環境

- **Container（容器）**：Image 執行後的實體執行實例

- **Dockerfile**：定義如何建構映像檔的腳本檔案

- **Volume**：用於容器資料的持久化與共用

- **Network**：容器間網路溝通配置（bridge / host / overlay 等）

- **Registry**：儲存映像檔的服務（如 Docker Hub）

## 基本操作流程

1. 撰寫 `Dockerfile` 或選擇現成的 Image

2. 使用 `docker build` 建立映像檔

3. 使用 `docker run` 啟動容器

4. 如需多服務整合，使用 `docker-compose` 編排

5. 推送映像至遠端 registry，如 Docker Hub / GitHub

## 筆記索引

- [[902.1-Dockerfile-語法與最佳實務]]
- [[902.2-docker-compose-進階用法]]
- [[902.3-VSCode-Remote Container 建置與應用]]
- [[902.4-Docker-資料持久化與 Volume 管理]]
- [[902.5-Docker-網路配置與容器溝通]]
- [[902.6-Docker-部署實戰與 AI 整合應用]]
- [[902.7-Docker-常見錯誤與除錯技巧]]

## 延伸閱讀

- [Docker 官方文件](https://docs.docker.com/)
- [Docker Hub](https://hub.docker.com/)
- [Awesome Docker](https://github.com/veggiemonk/awesome-docker)
- [[014.19-AI應用-模型部署與容器化 (Docker)]]
- [[014.20-AI應用-輕量模型與邊緣運算（Edge AI）]]