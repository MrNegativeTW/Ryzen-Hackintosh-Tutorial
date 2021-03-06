# 顯示 \(Nvidia\)

{% hint style="info" %}
Nvidia Web Driver 下載：[https://www.tonymacx86.com/nvidia-drivers/](https://www.tonymacx86.com/nvidia-drivers/)
{% endhint %}

## 安裝教學

### 找到版本並下載

從 Os Build 中的後綴號碼找到適合你系統的驅動並下載

例如筆者的是 macOS 10.12.6 Sierra **\(16G29\)**，就找到對應的版本下載

![](../.gitbook/assets/ying-mu-kuai-zhao-20180529-shang-wu-7.53.29.png)

### 安裝

毫無技術性，打開輸入密碼下一步案到底即可

### 啟用獨顯

正常來說應該會自己切換過去，如果沒有，記得切換過去

![](../.gitbook/assets/ying-mu-kuai-zhao-20180529-shang-wu-7.56.20.png)

### 如何確認獨顯已啟用？

打開「關於這台Mac」，顯示卡部分有正常列出型號及記憶體大小就表示啟用了！

勾了 重開機了 獨顯還是沒有接管嗎？

那就改Clover設定吧！

## 疑難排解

### 獨顯無法啟用？

打開 **Clover Configurator**

找到Boot，取消勾選 **nvda\_drv=1**

並到System Parameters勾選 **NvidiaWeb**

![nvda\_drv=1](../.gitbook/assets/nvdadrv.png)

![NvidiaWeb](../.gitbook/assets/nvidiaweb.png)

### 安裝後黑畫面？

Github Issue \#1

{% hint style="success" %}
\[Fix\] 10.12/10.13 Nvidia 2/3/4/5/6/7/9/10xx Series Black Screen

[https://www.tonymacx86.com/threads/fix-10-12-10-13-nvidia-2-3-4-5-6-7-9-10xx-series-black-screen.203430/](https://www.tonymacx86.com/threads/fix-10-12-10-13-nvidia-2-3-4-5-6-7-9-10xx-series-black-screen.203430/)
{% endhint %}

筆者的系統識別選擇了Mac Pro 5.1，所以在安裝上並無問題

![](../.gitbook/assets/3-1_5.png)

