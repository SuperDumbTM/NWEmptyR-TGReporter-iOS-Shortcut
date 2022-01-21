# NWmptyR-ios-shortcut

NWemptyR telegram 自20年尾開始全自動化（好似係），透過輸入特定格式文字作報料。<br>
而因為我嘅懶惰，於是用 Apple 嘅 [Shortcut](https://support.apple.com/zh-hk/guide/shortcuts/welcome/ios) 寫咗兩個 shortcut 嚟自動化報料嘅 process。<br>
亦都希望藉此令更加多人願意隨手報料。

## 下載
單一車站 EmptyR Report：
https://www.icloud.com/shortcuts/6832fbf9679446c7a3c8dd1041db37f8

多車站 EmptyR Report (Multi-Stat)：
https://www.icloud.com/shortcuts/52c549d340ab4158bbfba8d57a1543a2

(Last update: 2022-1-8)
- update prompt messages

## 點用﹖
**TLDR:** 好 straight forward 下，㩒下就識。
完全唔知 Shortcut 係咩嚟/點用請睇下[呢度](https://github.com/SuperDumbTM/EmptyR-ios-shortcut#shortcut-%E6%BA%96%E5%82%99)先

### - 單一車站 EmptyR Report

當㩒咗個 shortcut 後﹐程式會偵測你方圓100米內嘅車站，如果無嘅就會偵測方圓450米內嘅車站

**1. 方圓100米內只有一個車站**<br>
> ![sit1](https://user-images.githubusercontent.com/71750702/150392019-27f8f1b7-9a30-42a9-a82e-9c68d314a2dc.jpg)<br>
> 直接揀報咩料就可以


**2. 方圓100米內一個車站的冇，但450米內有**
> `No station detected`<br>
> 移動中嘅位置相比靜止誤差較大，所以亦使你就喺正個車站隔離都有機會<br>
> ![sit2](https://user-images.githubusercontent.com/71750702/150392033-bb446482-4076-4087-8e8a-0a47dd125a24.png)<br>
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
### - 多車站 EmptyR Report (Multi-Stat)
運作同上，但只報喜不報悲。出發車站、路線需要手動輸入，目的地車站自動偵測，乘車時間自動計算。<br>
![multi station](https://user-images.githubusercontent.com/71750702/150391418-305e7601-94ac-49ae-b1b4-89e529db0b39.png)
![multi route](https://user-images.githubusercontent.com/71750702/150391413-7cc02856-9b22-42a1-a01e-aad264d17ac1.png)

- 如果揀咗「手動輸入」，你需要手動輸入嗰程車嘅乘車時間（分鐘）<br>
![time](https://user-images.githubusercontent.com/71750702/150392234-d9235c89-fb78-4b2c-a5dd-034dbc59f23c.png)
![time tg](https://user-images.githubusercontent.com/71750702/150392237-10e98454-c3f9-4ec1-b864-291ba191d0d5.png)

- :warning: **如所選路線、上車車站及落車車站有衝突（所選路線不經上車/落車車站）**，行車時間即為0，姐係報料嘅上車時間=落車時間=當刻時間。**所以有轉車建議以最後乘搭路線作報料。**

---

**_車程計算方法_**
- ![time](https://user-images.githubusercontent.com/71750702/150392799-94c6cd10-5c1d-4908-ab7e-6373cf61de87.JPG)
- 上拾入
- 行車時間取自MTR

> Example (761P)<br>
> 全程行車時間：31 mins，全程車程數量：14個，站均行車時間：2.214 mins
> 天逸至康樂路 = 12個站，時間：26.571（= 27 mins）


## Shortcut 準備

### 準備
打開設定，碌落去揾 `Shortcut/捷徑`<br>
![setting shortcut](https://user-images.githubusercontent.com/71750702/150395397-113a9449-65ac-46d3-aa99-b584cb7d8c5c.JPG)<br>
開 `允許不受信任的捷徑`、`精確位置`<br>
![shortcut location](https://user-images.githubusercontent.com/71750702/150395543-f6beb365-c811-453a-a528-fac301028240.JPG)

### 加入捷徑
㩒咗下載嘅 link 之後理論上會見到呢個畫面<br>
改名可以噝綠圈位置改。<br>
![download](https://user-images.githubusercontent.com/71750702/150477941-b3a4a711-0a93-4bdb-bf38-13a202b3b0f9.JPG)<br>
剝到最底，㩒 `加入不受信任的捷徑`<br>

### Shoutcut 嘅 shortcut
下下要㩒入個shortcut app度就無咗原有方便嘅義意鳥。<br>
而Shortcut係可以加入主畫面的，方法有兩。

1. [Widget](https://support.apple.com/zh-tw/guide/shortcuts/apd029b36d05/ios)
2. App icon<br>
  首先打開捷徑app，揾返個shortcut㩒右上角嘅三粒點<br>
  ![app icon 1](https://user-images.githubusercontent.com/71750702/150481077-0d3ae6a2-8a93-41c1-901d-4282431fa287.JPG)<br>
  最㩒多次右上角三粒點<br>
  ![app icon 2](https://user-images.githubusercontent.com/71750702/150481327-22d52ce9-2e8c-48b6-98c4-fd2cf71aca2b.JPG)<br>
  改名、改icon、改顏色可以喺度改。<br>
  㩒 `加至主畫面` 你就會得到一粒 ”app” icon<br>
  ![app icon 3](https://user-images.githubusercontent.com/71750702/150483116-521a9786-4ca9-466c-b1eb-aaffccd234ed.JPG)

### 點用 shortcut

㩒返相應嘅widget/ app icon就用到。<br>
Shortcut讀取你嘅位置要5-10秒左右，所以會有一段時間冇任何反應。<br>
如果偵測位置過程熄咗mon都無問題的，只要㩒返個通知就可以繼續。<br>
![noti](https://user-images.githubusercontent.com/71750702/150483543-13134ba7-0dea-481e-b7fe-53f6b57ea10b.JPG)

