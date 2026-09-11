# PoseTwin v8.2.1 — GPU 狀態卡修正版

修正內容：

- GPU / Full 模型成功建立後：
  - 右上角狀態顯示「AI + 3D 骨骼已就緒（GPU / Full）」
  - 中間大卡片同步切換成「✓ 模型已就緒」
  - 顯示「已使用 GPU / Full 模型。現在可以上傳影片或開啟相機。」
- CPU / Lite 成功路徑已驗證，仍會正確顯示 ready。
- 保留 No-VRM、15 節段教學人偶架構。
- 不使用假的百分比進度。

部署：
用此版 `index.html` 覆蓋 GitHub Pages repository 根目錄的 `index.html`。
