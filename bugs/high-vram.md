# VRAM 使用率超高

## 症狀

裝了 iStat Menus 後，有觀察到剛開機時顯卡記憶體使用率超高，導致畫面 Lag，可是在睡眠喚醒後，使用率會降低到一半以下，直覺就是有東西卡住那些 VRAM

總之加了一個 Kext 和一些 Flags 後，這事就解決了

## 解法

### 加Kext

不意外的，就是 [NvidiaGraphicsFixUp](https://github.com/lvs1974/NvidiaGraphicsFixup/releases)

除了加 NvidiaGraphicsFixUp 之外，記得也要更新 Lilu 喔

{% hint style="info" %}
下載：[https://github.com/lvs1974/NvidiaGraphicsFixup/releases](https://github.com/lvs1974/NvidiaGraphicsFixup/releases)
{% endhint %}

安裝很簡單，就丟進 EFI/EFI/CLOVER/kexts/10.12

### Boot Flags

開啟 Clover Configurator，在 Boot 頁面中的 Custom Flags 加入

`-ngfxbeta`

`-ngfxgl=1`

`-ngfxcompat=1`

![](../.gitbook/assets/bootflags_nvidia.png)

## 後記

作者提供的 Flags 很多，我也試了很多，總之這樣搞之後 VRAM 使用率就下降了，目前使用上也沒什麼問題

