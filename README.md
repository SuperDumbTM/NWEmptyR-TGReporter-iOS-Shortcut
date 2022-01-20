# EmptyR-ios-shortcut

NWemptyR telegram 自20年尾開始全自動化，透過輸入特定格式文字作報料。<br>
而因為我嘅懶惰，於是用 Apple 嘅 [Shortcut](https://support.apple.com/zh-hk/guide/shortcuts/welcome/ios) 寫咗兩個 shortcut 嚟自動化報料嘅 process。<br>
亦都希望藉此令更加多人願意隨手報料。

## 下載
單一車站 EmptyR Report：
https://www.icloud.com/shortcuts/6832fbf9679446c7a3c8dd1041db37f8

多車站 EmptyR Report (Multi-Stat)：
https://www.icloud.com/shortcuts/52c549d340ab4158bbfba8d57a1543a2

(Last update: 2021-1-8)
- update prompt messages

## 點用﹖
**TLDR:** 好 straight forward 下，㩒下就識。
完全唔知 Shortcut 係咩嚟/點用請睇下[呢度](https://github.com/SuperDumbTM/EmptyR-ios-shortcut/blob/main/README.md#shortcut-%E6%BA%96%E5%82%99)先

### 單一車站 EmptyR Report

當㩒咗個 shortcut 後﹐程式會偵測你方圓100米內嘅車站，如果無嘅就會偵測方圓450米內嘅車站

**1. 方圓100米內只有一個車站**
> ![sit1](https://user-images.githubusercontent.com/71750702/150386083-22930509-71dd-4c9c-ab61-c47c31bf5f22.jpg)<br>
> 直接揀報咩料就可以


**2. 方圓100米內一個車站的冇，但450米內有**
> `No station detected`<br>
> 移動中嘅位置相比靜止誤差較大，所以亦使你就喺正個車站隔離都有機會
> ![sit2](https://user-images.githubusercontent.com/71750702/150387124-6b0184a5-a7bb-49a6-8627-15b06fe3271e.png)<br>
> 揀返啱嘅就OK

**3. 方圓100米內多於一個車站**
> `Multiple stations detected`<br>
> 有少數車站站距約等於100米，多數位於屯門區<br>
> 都係揀返啱嘅就OK

---

**_手動輸入_**
- 會自動喺 telegram 輸入 `時間 + dummy + #報料`
- 預設輸入 dummy 方便㩒兩下highlight改咗佢<br>

**_離開捷徑_**
- 字面意思，㩒空白位置同樣校果。

---
### 多車站 EmptyR Report (Multi-Stat)
運作同上。出發車站、路線需要手動輸入，目的地車站自動偵測，只報喜不報悲。<br>



## Shortcut 準備

