# PoseTwin v4 — 3D Skeleton

這一版把右側從「線條骨架」改成真正的立體骨骼視覺化。

## 新增
- 3D 圓柱骨段，不再是細線
- 球狀關節
- 3D 頭部與軀幹
- MediaPipe `worldLandmarks` 驅動
- 可拖曳旋轉 / 縮放 3D 視角
- 顯示 / 隱藏地面格線
- 自動旋轉
- 重置 3D 視角
- 前 / 後鏡頭切換
- 直接錄製右側 3D 骨骼 WebM
- 下載 3D 骨骼 PNG

## 部署
將新的 `index.html` 上傳至 GitHub `PoseTwin` repository 根目錄，覆蓋舊版檔案。

GitHub Pages 約數十秒到數分鐘後更新。

## 注意
此版本使用 Three.js 與 MediaPipe CDN，因此第一次開啟需要網路連線。
