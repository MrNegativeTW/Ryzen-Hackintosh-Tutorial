# 關於讀寫 NTFS

macOS 預設情況下，是無法對 NTFS 磁區進行寫入的，只能有讀取功能，而且有些檔案還會呈現灰色無法拉出使用...

## 解決辦法

安裝可以讀寫的程式，有兩個方案

方案一：Microsoft NTFS for Mac by Paragon Software

方案二：Mounty for NTFS

### 方案一

`付費方案`

{% hint style="info" %}
[https://www.paragon-software.com/home/ntfs-mac/](https://www.paragon-software.com/home/ntfs-mac/)
{% endhint %}

付錢解決，有錢人的做法，我們 ~~窮人~~ 開源節流的人是不會這樣的，不過經過試用，穩！

### 方案二

`免費方案`

{% hint style="info" %}
[https://mounty.app/](https://mounty.app/)
{% endhint %}

其實，macOS 內建是支援 NTFS 讀寫的，不過基於某種原因（不穩定，我猜）被鎖起來了，這套工具只是幫你把內建的功能打開，使用時還是小心為上

原本沒這套工具又要使用內建的讀寫時，需要手動重新掛載磁區，有夠麻煩， 所以這套工具就被開發出來，按一下即可自動幫你重新掛載

## **方案二的已知問題**

### 無法掛載

問題：隨身碟插入後無法掛載 或 電腦意外斷電後無法掛載磁區

解法：插上 Windows 的電腦並安全移除；重啟進入 Windows 然後再重啟進入 macOS

說明：請謹記，任何 NTFS 格式的裝置在前一台電腦必須是安全的被移除（也就是按下退出），否則都會無法掛載

### 檔案不見了

問題：對 NTFS 磁區進行操作時，突然間整個 資料夾 / 檔案 全部消失了

解法：

1. 開啟 Windows 並對磁區進行掃描與修復
2. 如果你手邊沒有 Windows，可以使用 [Paraogn Harddisk Manager](https://www.paragon-software.com/home/hdm-mac/) 或 [Tuxera Disk Manager](http://www.tuxera.com/products/tuxera-ntfs-for-mac/) 進行處理

### 檔案變灰色

問題：打開磁區一看，哇，檔案都是灰色的，複製也複製不出來，完全無法操作

解法：用終端機導航到檔案位置，並輸入 `ls -l@ <filename>`查看檔案額外的屬性，  
然後輸入  `xattr -d com-apple.<attribute> <filename>` 移除這些屬性，  
例如：`xattr -d com.apple.FinderInfo testfile.txt`

說明：據軟體說明頁面指出，這是因為檔案有一些延伸屬性，想情請見 [the Manpage of xattr](https://developer.apple.com/library/mac/documentation/Darwin/Reference/ManPages/man1/xattr.1.html) （頁面已被移除）

