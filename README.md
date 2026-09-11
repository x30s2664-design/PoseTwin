# PoseTwin v8 — VRM Humanoid

這一版把右側模型架構從自製幾何人偶升級為 Humanoid / VRM。

## 主要功能
- 預設載入 VRM Humanoid 人體。
- 使用 MediaPipe PoseLandmarker 驅動：
  - Hips / 骨盆
  - Spine / Chest / UpperChest
  - Head
  - 左右上臂、前臂
  - 左右大腿、小腿、腳
- 胸廓與骨盆分開驅動，轉身與扭腰比兩格圓柱更自然。
- 可自行上傳 `.vrm` 模型。
- VRM 載入失敗時，自動回退至原本 15 節段教學人偶。
- 保留影片上傳、相機、鏡像、慢速、逐格、正側面、錄製與截圖。
- 模型載入狀態不使用假的百分比。

## 預設 VRM
預設從 GitHub / jsDelivr 載入 madjin/vrm-samples 的 Avatar_Orion.vrm。
該 GitHub 專案將 Avatar Orion 列在可自由使用的 CC0 sample models 中。

## 部署
將 `index.html` 覆蓋 GitHub Pages repository 根目錄的 `index.html`。

## 注意
VRM 是外部網路資源；如果學校網路封鎖 jsDelivr，請使用「載入 VRM」選擇本機 `.vrm` 檔案，或切回「15 節段人偶」。
