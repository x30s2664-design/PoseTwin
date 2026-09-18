# EmbodiedSpace MVP v0.1

瀏覽器端「有限容量具身空間」分析原型，支援：

- 上傳照片
- 上傳影片逐幀分析
- 即時相機分析
- 即時分析畫面錄製（WebM）
- 多人 Pose（最多 6 人）
- 🔴 本體空間
- 🟡 非均質近體空間：臉/頭、手、腳較大；軀幹較小
- 🔵 有限遠體空間：只顯示有限外圍場，再外部環境不著色

## 啟動

直接部署到 GitHub Pages 即可。若本機測試相機，請使用 localhost HTTP server（例如 `python -m http.server 8000`），不要直接以 `file://` 開啟。

## 模型說明

部位權重是研究模型參數，受 cortical homunculus 概念啟發，不應被解讀為直接的生理或臨床測量值。
