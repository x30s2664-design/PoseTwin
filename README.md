# PoseTwin v2

功能：
- 上傳本機影片
- 直接開啟 Webcam
- 左右雙螢幕：原始影像 / AI 骨骼
- 同步播放與時間軸
- 直接錄製右側骨骼 Canvas
- 停止後下載 WebM
- 下載骨骼 PNG 截圖
- 純前端，可部署 GitHub Pages

## 部署
把 `index.html` 上傳到 GitHub repo 根目錄後，在 Settings → Pages：
- Deploy from a branch
- Branch: `main`
- Folder: `/ (root)`

## 注意
相機功能需要 HTTPS；GitHub Pages 預設符合需求。
第一次使用需允許相機權限並連線下載 MediaPipe 模型。
