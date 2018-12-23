# 關於顯卡性能損失

目前爬文結果表示，Ryzen 配上 Nvidia 的顯卡，性能損失約50%，配上 AMD 的顯卡，大約10%

筆者使用 Ryzen + 1050，像是 Mission Control 之類的都會小Lag

筆者朋友使用 Intel + 660，順暢無誤

所以如果可以，上 A 卡吧，只要放個 WhateverGreen 跟加入 bootflag 就可正常

總之我們就來實測一下，**全部預設，沒有超頻**

## Ryzen 7 1700 + GTX 1050

### Windows

可以看到正常效能應該落在 **87fps** 附近

> R15辨識有問題，變成Windows 8了

![](../.gitbook/assets/wei-ming-ming.png)

### macOS

可是同樣配備到了 macOS 卻剩下 43fps

![](../.gitbook/assets/r15.png)

## Ryzen 7 1700 + RX460

### Windows

可以看到正常效能應該落在 **83fps** 附近

![](../.gitbook/assets/rx460_win.png)

### macOS

可是同樣配備到了 macOS 卻剩下 70fps \(第一次 74，第二次 71，這是第三次成績\)

![](../.gitbook/assets/rx460_macos.png)

## 同場加映

### Windows - i7 4770 + GT730 \(8G RAM / 學校電腦\)

就連 GT730 這張卡都有 65fps 啊啊啊啊

![](../.gitbook/assets/gt730.png)

### Windows - AMD FX-8100 + HD7730 \(8G RAM / 路邊撿到的電腦\)

![](../.gitbook/assets/r15.PNG)

