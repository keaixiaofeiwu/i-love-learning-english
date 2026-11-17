# 我愛學英文

自製英語教學影片收藏網站，提供影片搜尋、主題分類、YouTube 播放、學習重點與隨堂練習。

目前網站：https://after-class-english-films.workspace-395034.chatgpt.site

網站目前僅擁有者可觀看，需登入原網站擁有者的 ChatGPT 帳號。這個 GitHub 儲存庫用於保存網站原始碼，未啟用公開的 GitHub Pages。

## 檔案

- `index.html`：網站首頁，包含樣式與互動程式。
- `videos.json`：教學影片清單。
- `participial-showreel.html`：分詞構句互動教學，內嵌旁白、動畫與錄影功能。
- `PUBLISHING.md`：影片歸檔與網站維護流程。

## 本機預覽

在此目錄啟動靜態 HTTP 伺服器，再開啟 localhost 網址。例如已安裝 Python 時：

```sh
python -m http.server 8000
```

直接用 `file://` 開啟首頁時，瀏覽器可能禁止載入 `videos.json`。互動教學單檔可獨立開啟。

## 新增影片

在 `videos.json` 新增一筆影片資料，沿用現有欄位，包含唯一 id、標題、分類、YouTube ID、Google Drive 原檔連結及學習重點。驗證畫面與連結後，更新目前的 Sites 私人網站部署。

影片 MP4 原檔存放於 Google Drive，不將影片二進位檔加入 Git 儲存庫。

本專案未授予開放原始碼授權；未經擁有者同意，不得另行散布影片或素材。
