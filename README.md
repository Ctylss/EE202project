📁 專案目錄結構說明 1
csharp

```

project/                     # 專案根目錄
├── backend/                 # 後端專案 (Spring Boot)
│   ├── .mvn/                # Maven Wrapper，用於統一 Maven 版本
│   ├── .vscode/             # VS Code 編輯器設定
│   ├── src/                 # 原始碼目錄
│   │   ├── main/            # 主要應用程式程式碼
│   │   │   ├── java/
│   │   │   │   └── com.project.backend/         # 主套件 (Package)，遵循反向域名慣例
│   │   │   │       ├── controller/              # 控制器層：處理 HTTP 請求，協調業務邏輯
│   │   │   │       ├── dao/                     # 資料存取層：處理資料庫 CRUD 操作
│   │   │   │       ├── model/                   # 模型層：定義資料結構與實體
│   │   │   │       ├── service/                 # 服務層：實作核心業務邏輯
│   │   │   │       ├── util/                    # 工具類別：存放通用輔助函數
│   │   │   │       └── BackendApplication.java  # 應用程式啟動主類別
│   │   │   └── resources/
│   │   │       ├── application.properties/yml   # 應用程式主要設定檔
│   │   │       ├── static/                      # 靜態資源 (不建議，除非有特定需求)
│   │   │       └── templates/                   # 網頁模板 (若有後端渲染頁面)
│   │   └── test/                                # 測試程式碼目錄
│   ├── .gitignore           # Git 忽略提交檔案設定
│   └── pom.xml              # Maven 專案管理檔，定義依賴與建置配置
│
└── frontend/                # 前端專案 (Vue.js)
    ├── node_modules/        # 存放 npm 安裝的第三方函式庫
    ├── public/              # 存放靜態資源，例如 index.html, favicon
    ├── src/                 # 原始碼目錄
    │   ├── assets/          # 靜態資源，如圖片、字體、全域 CSS
    │   ├── components/      # 可重用的 UI 組件
    │   │   ├── base/        # 基礎組件 (如：按鈕、輸入框)
    │   │   └── common/      # 通用組件
    │   ├── router/          # Vue Router 設定，管理所有頁面路由
    │   ├── services/        # 與後端 API 互動邏輯
    │   │   └── api.js       # 處理資料請求與響應的通用方法
    │   ├── store/           # Vuex 或 Pinia 狀態管理
    │   ├── utils/           # 通用工具函數 (如：日期格式化、表單驗證)
    │   ├── views/           # 頁面級組件，透過路由切換
    │   │   ├── HomeView.vue # 首頁
    │   │   └── LoginView.vue# 登入頁
    │   └── App.vue          # 應用程式的根組件
    ├── .gitignore           # Git 忽略提交檔案設定
    └── package.json         # npm 專案管理檔，定義依賴與腳本
```
