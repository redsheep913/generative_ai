# Generative AI
# HW1

## About this project

請在colab中畫一個函數圖形。

繳交期限：3/10 23:59

### 繳交標題格式：

學校 學號 系級 姓名 主題 (主題可打可不打)(學校、系級打簡稱即可)

### 繳交內容必須包含：

1. colab連結(請記得將共用權限打開)
2. 對此份作業的重點說明
3. 此份作業的重點截圖

### 評分標準：

- 0分：程式連結無法順利開啟，且無截圖。
- 1分：程式開啟後只有匯入基本套件。
- 2分：程式連結無法順利開啟，但有部份截圖。
- 3分：繳交作業與本周主題無關(若貼成別週作業也列在此。)
- 6分：作業繳交基本分，程式內容與課堂範例十分近似。例如sin(x)改成cos(x)或2sin(x)。
- 8分：常見一元二次函數。
- 9分：圖形很有創意(本週老師沒教到的函數都可以)。
- 10分：圖形很有創意、且有漂亮文字註解 (Markdown)。
- 註一：若沒有引入老師的固定4行套件，總分 -1。
- 註二：程式連結無法順利開啟包含 1.權限未開啟 2.繳交非colab連結的檔案 3.程式碼無法完整執行

---

以下為繳交作業內容：

# **台師大 61347058S 資工碩一 宋宏洋 第一週作業02/18**

### Colab連結

[Google Colab](https://colab.research.google.com/drive/1hXuQQaob00uGSbdw1H35ApeZHSDexmyf#scrollTo=lf0Vqi4ACUIN)

1. 畫出y=cos(x)圖形, 一元二次式

2. 畫出右半邊的愛心圖形

### 函式庫使用

- numpy: 用於數值計算和陣列操作
- matplotlib.pyplot: 用於繪製圖形

### 資料準備

- 使用 `np.linspace(-2, 2, 400)` 建立 x, y 座標點
    - 範圍: -2 到 2
    - 取樣點數: 400 個點
- 使用 `np.meshgrid()` 建立二維網格
    - 將一維的 x, y 陣列轉換成二維網格座標系統
    - X, Y 分別代表網格上每個點的 x, y 座標值

### 方程式定義

- 原方程式: `x^2 + (y - x^(2/3))^2 = 1`
- 程式中表示為: `Z = X**2 + (Y - X**(2/3))**2 - 1`
    - `*` 表示次方運算
    - 將等式移項後，左邊為 Z，右邊為 0

### 繪圖設定

- 使用 `plt.contour()` 繪製等高線圖
    - `levels=[0]`: 只畫出 Z=0 的等高線，即原方程式的解
    - `colors='darkred'`: 設定線條顏色為深紅色
- 加入座標軸標籤和標題
    - `xlabel`: x 軸標籤
    - `ylabel`: y 軸標籤
    - `title`: 圖形標題
- 使用 `plt.grid(True)` 加入網格線增加可讀性

### 輸出結果

- `plt.show()` 顯示最終圖形
- 圖形會呈現出一個特殊的曲線，這是原方程式在 x-y 平面上的軌跡

https://cool.ntu.edu.tw/users/232372/files/7054669/preview?verifier=pUrXknKY7lOkA6uPah8pSxhEs4haDTMiA92FcoL6

https://cool.ntu.edu.tw/users/232372/files/7054666/preview?verifier=uRDKGm3bmueUlhtrb3DAo1q7Q7ScnDBQVXnttDlN

https://cool.ntu.edu.tw/users/232372/files/7054601/preview?verifier=owH0TnB4M5qwInsxjabpsShtOOs3ltTJib6CKgfn