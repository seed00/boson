# i1旋鈕模組

## 實體照片

![](../../.gitbook/assets/rotation_sensor.jpg)

## 基本信息

中文名稱：旋鈕模組

英文名稱：Rotation Sensor

編號：i1

SKU：BOS0001

## 功能簡介

旋鈕模組是基於電位器的旋轉角度感測器，旋轉角度從0到300度，可以非常容易地實現與旋轉位置相關的互動效果。旋鈕可廣泛應用於調速風扇、換擋汽車、家用洗衣機等。這是一款非常基本的類比訊號輸入裝置，你可以通過它來學習類比訊號的處理，進而學習更多類比感測器。

![](../../.gitbook/assets/rotation_sensor_intro.png)

## 使用說明

旋鈕模組上帶有旋轉箭頭標識，在使用時通過調節旋鈕角度即可控制類比訊號輸入的大小。以旋鈕控制風扇為例：

> * 順時針旋轉代表類比訊號增強，風扇會轉得愈來愈快；逆時針旋轉代表類比訊號減弱，風扇會變慢。

![](../../.gitbook/assets/rotation_sensor_ui.png)

## 原理介紹

旋鈕模組通過調節旋鈕，在一定範圍內改變電阻值，從而改變輸出訊號的大小。

## 實作範例教學-基本篇

### 變速風扇

**範例說明：**通過轉動旋鈕到不同的角度來控制風扇轉動速度。順時針旋轉，風扇轉速增大；逆時針旋轉，風扇轉速降低。

**元件清單：**旋鈕模組；風扇模組；主控板：3組輸入/輸出端。

**連線圖：**

![](../../.gitbook/assets/rotation_sensor_example1.png)

### 調速打蛋器

**範例說明：**製作一個打蛋器，打蛋器的打蛋頭固定在馬達的轉軸上，使用旋鈕模組控制馬達的轉速。

**元件清單：**旋鈕模組；馬達模組；主控板：1組輸入/輸出端。

**連線圖：**

![](../../.gitbook/assets/rotation_sensor_example3.png)

## 實作範例教學-Micro:bit篇

### \(2\) 旋鈕檯燈

**範例說明：**使用旋鈕控制LED燈模組的亮度。順時針轉動旋鈕，LED燈模組越來越亮，逆時針轉動旋鈕，LED燈模組越來越暗。

**元件清單：**旋鈕模組；LED燈模組；Micro:bit；Micro:bit BOSON 擴充板。

**連線圖：**將旋鈕模組連接至Micro:bit擴充板的P0腳位，LED燈模組連接到Micro:bit擴充板的P8腳位。

![](../../.gitbook/assets/rotation_sensor_example2.png)

**程式說明：**① 讀取P0腳位的類比值；② 將讀取到的類比值賦給P8腳位。

**程式示意圖（中文版）：**

![](../../.gitbook/assets/rotation_sensor_prg_ch_tw.png)

**Example program\(English\):**

![](../../.gitbook/assets/rotation_sensor_prg_en%20%281%29.png)

## 商品規格

腳位說明：

![](../../.gitbook/assets/rotation_sensor_spec%20%281%29.png)

| **編號** | **名稱** | **功能說明** |
| :---: | :---: | :---: |
| 1 | GND | 電源接地 |
| 2 | VCC | 電源正極 |
| 3 | A | 類比訊號 |

重量： （g）

尺寸：26mm\*22mm

工作電壓：3.0-5.5V

工作電流：\(Max\)1mA@5V
