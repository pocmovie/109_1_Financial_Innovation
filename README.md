# 109_1_Financial_Innovation

## HW1

### 在util_pattern.py中：
* end_idx判斷式bug-fixed。  

### 在Detect.py中：  
* 用條件較為寬鬆的"Dark Cloud Cover"和"Piercing Pattern"取代類似的"Bearish Engulfing"和"Bullish Engulfing"。
* 類似"Evening/ Morning Star"和較為嚴苛，第九根為doji的"Bearish/ Bullish Abandoned Baby"的關係。

## HW2

### Candlestick Classification
* Model Accuracy都高於80%。

### 針對LSTM有嘗試進行Dropout，討論如下：
* 加入Dropout層的結果沒有比較好，最佳在49 iter, with 80.3% Accuracy。
* 原本的LSTM可能有overfitting的問題：  
  - 然因Eur/ Usd算穩定，若沒有劇烈匯率變化，在預測未來資料的Candlestick型態上便沒有問題。  
  - 若匯率有較大變化，便應該先按時間前後切資料，再進行Shuffle，以進一步驗證是否有overfitting。  

### 針對CNN討論如下：
* 在10個iter下，CNN的預測能力明顯好於預測Sequential的LSTM。
* 如同MNIST資料集，因CandleStick應該也是電腦看得懂的視覺資料。

## 期末報告
* Youtube連結如右：
