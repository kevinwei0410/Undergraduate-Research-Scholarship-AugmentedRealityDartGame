# 🏹 應用深度學習 & 特徵點辨識技術之擴增實境標靶遊戲

## 📌 摘要
在以往，玩射飛鏢需要有標靶跟飛鏢等器材，且受到空間限制，需在足夠大的空間讓玩家投擲飛鏢。本專題主要朝向創造**不受空間與器材限制，且具備高度即時性**的手機遊戲，以貼近實際射飛鏢情境。

為達到不受器材限制，本專題運用 **擴增實境 (AR) 技術**，在手機相機畫面上繪製**虛擬標靶與虛擬飛鏢**。標靶透過 **特徵點辨識技術** 進行定位，以獲取標靶與手機的相對位置。

發射虛擬飛鏢的方式，透過 **CNN 訓練神經網路模型辨識發射手勢**，並利用 **LSTM 判斷發射速度**。為確保高即時性，將神經網路模型**部署於伺服器端**，並透過 **GPU 加速運算**。手機端將相機影像傳輸至伺服器進行處理，計算後回傳發射參數至手機端。

透過上述設計流程與架構，成功實作此系統，使其能在 **實境影像上繪製虛擬標靶與飛鏢**，並透過 **手勢決定發射飛鏢及其初速 (m/s)**，飛鏢發射後的**飛行軌跡** 也能清楚呈現在遊戲畫面中。每個 **frame** 在伺服器端從 **解碼影像到神經網路模組偵測** 耗時約 **0.1 秒**，無明顯延遲，提供流暢的遊戲體驗。

---

## 🔑 關鍵字
- **擴增實境 (AR)**
- **特徵點辨識**
- **即時影像傳輸**
- **神經網路**


---

## 👥 四人分工
- 🎨 **前端UI 設計與標靶飛鏢建模**（手機 APP、AR 物體建模）:羅Ｏ
- 🌐 **網路設計**（手機與後端對接、多⼈遊戲對接）:李Ｏ
- 🏹 **飛鏢物理引擎**（重力計算、飛鏢路徑）：洪Ｏ洋
- 🧠 **後端神經網路辨識**（包含高解析神經網路、CNN-based特徵擷取網路、LSTM 動作辨識網路):魏Ｏ碩

---

## 📑 報告文件
- **📘 組別報告:** [🔗 點此查看](https://drive.google.com/file/d/1PHsOAP4BDYN_QiMHhDTvzju7SSnyQUmw/view?usp=sharing)  
- **📗 魏Ｏ碩個人報告（後端-神經網路高解析與辨識）:** [🔗 點此查看](https://drive.google.com/file/d/1eAMZauSMhtNTEae4AX0CaJ-Vt5Q4fNzs/view?usp=sharing)

---
