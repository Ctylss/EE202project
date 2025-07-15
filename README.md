# EE202project

2025/7/15

project/ # 專案根目錄
├── backend/ # 後端專案 (Spring Boot)
│ ├── .mvn/ # Maven Wrapper
│ ├── .vscode/ # VS Code 專屬設定
│ ├── src/ # 原始碼目錄
│ │ ├── main/ # 主要程式碼
│ │ │ ├── java/ # Java 程式碼
│ │ │ │ └── com.project.backend/ # 主套件 (Package)
│ │ │ │ ├── controller/ # 處理 HTTP 請求，回傳 JSON
│ │ │ │ ├── dao/ # 資料庫存取層，處理資料增刪改查
│ │ │ │ ├── model/ # 資料模型，與資料庫表格對應
│ │ │ │ ├── service/ # 業務邏輯層，協調 controller 與 dao
│ │ │ │ ├── util/ # 通用工具類別，例如日期處理
│ │ │ │ └── BackendApplication.java # 應用程式啟動主類別
│ │ │ └── resources/ # 設定檔與靜態資源
│ │ │ ├── application.properties/yml # 應用程式主要設定檔
│ │ │ ├── static/ # 靜態資源 (不建議，除非有特定需求)
│ │ │ └── templates/ # 網頁模板 (如果後端有渲染頁面)
│ │ └── test/ # 測試程式碼
│ ├── .gitignore # Git 忽略提交檔案
│ └── pom.xml # Maven 專案設定檔 (依賴管理)
│
└── frontend/ # 前端專案 (Vue.js)
├── node_modules/ # 存放第三方函式庫
├── public/ # 存放靜態資源，例如 index.html, favicon
├── src/ # 原始碼目錄
│ ├── assets/ # 存放靜態資源，例如圖片、字體、全域 CSS
│ ├── components/ # 存放可重用的 UI 組件 (按鈕, 導航欄等)
│ │ ├── base/ # 基礎組件
│ │ └── common/ # 通用組件
│ ├── router/ # Vue Router 設定，管理所有頁面路由
│ ├── services/ # 封裝與後端 API 互動的邏輯
│ │ └── api.js # 處理資料請求與響應
│ ├── store/ # Vuex 或 Pinia 狀態管理，類似後端的資料中心
│ ├── utils/ # 存放通用工具函數 (格式化、驗證等)
│ ├── views/ # 存放頁面級組件 (透過路由切換的頁面)
│ │ ├── HomeView.vue # 首頁
│ │ └── LoginView.vue# 登入頁
│ └── App.vue # 應用程式的根組件
├── .gitignore # Git 忽略提交檔案
└── package.json # npm 專案設定檔 (依賴與腳本)
