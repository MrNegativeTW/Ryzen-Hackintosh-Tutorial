---
description: 沒錢買Mac，所以買了Ryzen裝黑蘋果
---

# AMD Ryzen 安裝黑蘋果教學

{% hint style="success" %}
本教學撰寫進度 99%，最後更新日：2019 年 06 月 20 日 / 15:00
{% endhint %}

{% hint style="danger" %}
1. 建議不要把 AMD 裝黑蘋果拿來當你吃飯的工具，不然光 Debug 就飽了，要吃飯，推 Intel + nVidia 平台。
2. 本文以我的硬體出發，請自行確認您的硬體，不同的硬體有不同的驅動、內核等
{% endhint %}

{% hint style="info" %}
預計 2019 年 7 月安裝 macOS Mojava 10.14

安裝完成後這邊將不會再更新，反之會開一個新的 GitBook 紀錄 Mojave 安裝教學。
{% endhint %}

## 關於

由於安裝時遇到了非常多的阻礙，爬文爬遍了，例如 AMD OS X**、**r/hackintosh、Tonymacx86 等，所以在裝的時候就有個念頭：

> 我要寫一篇「從我的硬體出發，從系統到驅動安裝的黑蘋果教學文」

總之，歡迎分享本文，附上來源即可。

## 開 Issue

安裝有問題？開 Issue  
教學有問題？開 Issue  
教學需補充？開 Issue

撰寫於 [GitBook](https://mtwstudio.gitbook.io/ryzentosh) 上，同步於 [Github](https://github.com/MrNegativeTW/Ryzen-Hackintosh-Tutorial)

## 小問題

目前使用上遇到的小問題：

#### 日常

* 畫面有時小 Lag，詳見「顯卡性能損失」

#### 開發

* Android  檔案傳輸應用程式無法讀取我的手機，但用 Android Studio 開發時可正常測試 \(via ADB\)。
* Android Emulator 無法執行，會顯示未支援 SVM，用實機解決。
* XCode 執行一切正常，就只有 Simulator 會小 Lag
* XCode 版本太舊，僅能支援到 Swift 4.0，Simulator 最新只能到 11.2
* XCode 接實機測試時需要下載新版 DeviceSupport，除非你的實機是舊版。
* XAMPP 不能安裝帶有 **VM** 字樣的版本，下載時請注意

## 關鍵字

Ryzen 安裝黑蘋果  
AMD 黑蘋果  
Ryzen 黑蘋果教學  
Ryzen 黑蘋果  
Ryzen 7 1700 黑蘋果   
RX460 黑蘋果  
AB350 Gaming3 黑蘋果  
GTX1050 黑蘋果

## 

```python
# Joke.py
while (AMD + Hackintosh) == 1:
    Debug()
```









