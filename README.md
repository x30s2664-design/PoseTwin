# PoseTwin v4.1 — MediaPipe 修復版

這版針對畫面出現「模型載入失敗」進行修復。

## 主要修正

- MediaPipe Tasks Vision 改用穩定版 `1.0.1`
- WASM 路徑固定為 `@mediapipe/tasks-vision@1.0.1/wasm`
- Pose model 改用固定版本 `/float16/1/`，不使用 `latest`
- 優先 Full + GPU
- GPU / Full 初始化失敗時，自動改用 Lite + CPU
- 頁面新增「↻ 重試模型」
- 頁面顯示實際初始化錯誤，方便手機除錯
- 保留 3D 圓柱骨段、球狀關節、3D 視角、前後鏡頭、錄影與下載

## 更新 GitHub Pages

1. 解壓縮 ZIP。
2. 將新的 `index.html` 上傳到 PoseTwin repository 根目錄。
3. 覆蓋舊版 `index.html`。
4. Commit changes。
5. 等待 GitHub Pages 重新部署。
6. 手機重新整理；若仍看到舊版，可使用無痕視窗測試。

## 正常狀態

右上角應顯示其中一種：

- `AI + 3D 骨骼已就緒（GPU / Full）`
- `AI + 3D 骨骼已就緒（CPU / Lite）`

播放影片後右側 FPS 會開始變動並顯示 3D 骨骼。
