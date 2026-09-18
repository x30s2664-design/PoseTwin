# EmbodiedSpace v0.2

改版重點：
- 33 點 MediaPipe Pose Landmarker Full。
- 開啟 `outputSegmentationMasks`，優先以人體 segmentation 畫本體空間。
- 無 segmentation 時才用 33 點重建身體 mask。
- PPS 沿人體輪廓建立，不再用人物外接框或大圓。
- 臉、手、腳加權較大；軀幹與肢段較小。
- 遠體空間只是一個有限外圈，不是整張畫面。
- 支援照片、影片、相機即時分析與分析畫面錄製。
