# Adobe 系列崩潰問題

## 症狀

| 軟體版本 | 症狀 | 解決辦法 |
| :--- | :--- | :--- |
| Premiere Pro CC 2018 | 貌似正常，除加入防手震會崩潰 | 無 |
| After Effects CC 2018 | 連開都打不開 | 指令 |
| Photoshop CC  2018 | 2018打不開，2017選字崩潰 | 指令 |
| illustrator CC 2018 | 打不開 | 指令 |
| illustrator CC 2017 | 打不開 | 指令 |
| Lightroom CC | 打不開 | **降版裝** |

## 解法

### After Effects CC 2018

sudo rm -rf /Library/Application\ Support/Adobe/Plug-Ins/CC/File\ Formats/Camera\ Raw.plugin

### Photoshop CC 2018

sudo rm -rf /Applications/Adobe\ Photoshop\ CC\ 2018/Adobe\ Photoshop\ CC\ 2018.app/Contents/Required/Plug-ins/Extensions/FastCore.plugin /Applications/Adobe\ Photoshop\ CC\ 2018/Adobe\ Photoshop\ CC\ 2018.app/Contents/Required/Plug-ins/Extensions/MMXCore.plugin

### Illustrator CC 2018

rm -rf /Applications/Adobe\ Illustrator\ CC\ 2018/Adobe\ Illustrator.app/Contents/MacOS/MMXCore.plugin  /Applications/Adobe\ Illustrator\ CC\ 2018/Adobe\ Illustrator.app/Contents/Required/Plug-ins/Text\ Filters/TextModel.aip

### Illustrator CC 2017

rm -rf /Applications/"Adobe Illustrator CC 2017"/"Adobe Illustrator.app"/Contents/Required/Plug-ins/"Text Filters"/TextModel.aip

## 已知缺陷

### After Effects CC 2018

* 加入防手震會崩潰

### Photoshop CC 2018

* 調整影像有些還是會崩潰

### Illustrator CC 2018

* 未知

### Illustrator CC 2017

* 未知

### Lightroom CC 2015

* 使用臉孔偵測時會崩潰

