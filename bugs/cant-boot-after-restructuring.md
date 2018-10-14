# 在 Ｗindows 磁碟重組後無法開機

{% hint style="success" %}
原文：[https://www.tonymacx86.com/threads/solved-sudden-unable-to-boot.236168/](https://www.tonymacx86.com/threads/solved-sudden-unable-to-boot.236168/)
{% endhint %}

一次開進 Windows 後進行時碟重組，不過重組的是 E，完全跟 macOS 安裝的硬碟不相干

錯誤訊息如下

```text
** The volume Mac os Sierra could not be verified completely.
<Emergency>: Boot task failed: fsck-safe
```

## 解法

開機進入 Single User Mode，並且輸入以下指令， diskXsX 請替換為 macOS 所在地

```text
fsck_hfs -Rc -d /dev/diskXsX
```

## 如何進入Single User Mode

於 Clover 開機選單中按下**空白鍵**

並且選擇 **Single User Mode** ，然後選擇「使用這些選項開機」



