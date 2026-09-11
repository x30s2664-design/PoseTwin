# PoseTwin v9.0.1 — 3D 人偶無法建立修正版

## 根因
v9.0 在把單人狀態改成多人 Track 狀態時，誤刪了兩個必要的共用函式：

- `unitFrom(a,b,fallback)`
- `bounded(v,lo,hi)`

所以 AI 模型本身可以成功載入，但只要偵測到人體、開始建立 3D 人偶，就會出現 JavaScript ReferenceError，右側看不到模型。

## 修正
- 恢復 `unitFrom()`
- 恢復 `bounded()`
- 保留最多 3 人與獨立 Track
- runtime error 會直接顯示在頁面診斷區
- JavaScript 語法檢查通過
