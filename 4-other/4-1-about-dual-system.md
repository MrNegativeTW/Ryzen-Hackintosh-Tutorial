# 關於雙系統

雙系統安裝非常神奇，有兩種方法

1. Boot Camp
2. 直接裝

我個人採用第二種方法，直接裝！

安裝前請拔除所有硬碟，唯獨留下要安裝 Windows 的硬碟

安裝完成後將所有硬碟插回，並至 Bios 將開機順序改為使用 Clover 開機，Clover很聰明的，會自動抓取可開機磁區，這時候剛剛裝好的 Windows 會顯示出來了



不過不過，Clover會抓到非常多磁區，所以請依照個人狀況將其他磁區隱藏

Boot Windows from \[磁區代號\]，於 Clover Configurator 輸入這個代號就對了

![](../.gitbook/assets/4-1_1.png)

