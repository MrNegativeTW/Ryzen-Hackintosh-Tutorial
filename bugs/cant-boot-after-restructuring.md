# 在Ｗindows磁碟重組後無法開機

{% hint style="success" %}
原文：[https://www.tonymacx86.com/threads/solved-sudden-unable-to-boot.236168/](https://www.tonymacx86.com/threads/solved-sudden-unable-to-boot.236168/)
{% endhint %}

一次開進Windows後進行時碟重組，不過重組的是E，完全跟macOS安裝的硬碟不相干

錯誤訊息如下

```text
** The volume Mac os Sierra could not be verified completely.
<Emergency>: Boot task failed: fsck-safe
```

## 解決辦法

開機進入Single User Mode，並且輸入以下指令，diskXsX請替換為macOS所在地

```text
fsck_hfs -Rc -d /dev/diskXsX
```

## 如何進入Single User Mode

於Clover開機選單中按下**空白鍵**

並且選擇**Single User Mode**，然後選擇「使用這些選項開機」



