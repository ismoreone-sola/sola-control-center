# Sola Control Center 🦞

整合型 AI 工具儀表板

## 功能

- 🏠 **首頁** - 快速入口
- 🏢 **像素辦公室** - Star Office UI (需後端)
- 📝 **Sola 記事本** - 語音快速記錄

## Zeabur 部署

### 方法一：靜態網站 + 後端服務

1. 將此倉庫連接到 Zeabur
2. 添加服務：
   - **靜態網站**：服務 `dashboard.html`
   - **Python 服務**：運行 Star Office UI 後端 (端口 18791)

### 方法二：分開部署

- **主 Dashboard**：部署此倉庫
- **像素辦公室**：部署 [ringhyacinth/Star-Office-UI](https://github.com/ringhyacinth/Star-Office-UI)

## 開發

```bash
# 本地運行
python3 -m http.server 8080
# 訪問 http://localhost:8080/dashboard.html
```

## 目錄結構

```
├── dashboard.html          # 主控制台
├── public/
│   └── sola-note/         # Sola 記事本
└── README.md
```
