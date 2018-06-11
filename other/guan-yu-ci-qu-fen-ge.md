# 關於磁區分割

這是我的磁區分割現況

Kingston UV400 供 macOS使用 / HFS+

WD Green 120G 供 Windows 使用 / NTFS

WD Blue 1TB \(7200RPM\) 供儲存資料使用 / 分割為 exFAT + NTFS

## exFAT + NTFS有什麼好處？

這樣一來，exFAT的磁區就能在雙系統中存取了，不然macOS不支援NTFS，完全不能寫入

## 如何分割？

{% hint style="danger" %}
分隔前請備份好資料！
{% endhint %}

於macOS中打開磁碟工具程式

![&#x78C1;&#x789F;&#x5DE5;&#x5177;&#x7A0B;&#x5F0F;](../.gitbook/assets/ying-mu-kuai-zhao-20180528-xia-wu-6.57.57.png)

選擇你要的磁區，並按下清除

![&#x9078;&#x64C7;&#x78C1;&#x5340;](../.gitbook/assets/ying-mu-kuai-zhao-20180528-xia-wu-6.59.28.png)

格式選擇**ExFAT**

![ExFAT](../.gitbook/assets/ying-mu-kuai-zhao-20180528-xia-wu-7.00.34.png)









