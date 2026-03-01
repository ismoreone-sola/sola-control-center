# Sola Studio 🦞

整合型 AI 工具儀表板

## 功能

- 📝 **Sola 記事本** - 語音即時記錄，捕捉每個靈感瞬間
- 🏢 **像素辦公室** - AI 工作狀態看板（需後端服務）

## 訪問

- 首頁：https://solastudio.zeabur.app
- 記事本：https://solastudio.zeabur.app/note.html
- 辦公室：https://solastudio.zeabur.app/office.html

## 部署

### 靜態網站 (Zeabur)
1. 連接 GitHub 倉庫到 Zeabur
2. 選擇 Static 類型
3. Build Command: 留空
4. Output Directory: `./public`

### 後端服務 (像素辦公室需要)

#### Zeabur 部署
1. 在 Zeabur 專案中添加 **Python** 服務
2. 連接同一個 GitHub 倉庫
3. Build Command: `pip install -r requirements.txt`
4. Start Command: `python app.py`
5. Port: `18791`

#### 本地運行
```bash
cd backend
pip install -r requirements.txt
python app.py
# 訪問 http://localhost:18791
```

## 開發

```bash
# 本地運行靜態網站
python3 -m http.server 8080
# 訪問 http://localhost:8080
```

## 目錄結構

```
├── index.html          # 首頁
├── note.html           # 記事本
├── office.html         # 辦公室入口
├── star-office.html    # 像素辦公室
├── public/
│   ├── sola-note/     # 記事本資源
│   └── star-office/   # 像素辦公室資源
└── backend/
    ├── app.py         # 後端服務
    └── requirements.txt
```

## 版本

v2.0
