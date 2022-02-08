# Mask-test 簡易口罩測試&及時通知

https://user-images.githubusercontent.com/99164823/152931854-b53d4934-65e7-4885-bd52-8b110157e5fa.mp4



模型使用yolov5內建模型yolov5s.py作為訓練，數據集則是從網路上找有戴/無戴口罩的人臉照片各500張進行測試，最後再結合line.py到detect.py中作推播通知

# 使用方法
準備好數據集資料後，執行train.py進行訓練，訓練後的結果會保存到指定路徑的run/test資料夾下，每次訓練結束會保存best.pt和last.pt兩個模型，訓練完之後，使用best.pt進行測試得到最佳的模型後，執行detect.py進行辨識，得到結果為沒有戴口罩，line則會傳送通知警告。
