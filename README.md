# SnapSleep
Where the SLEEP begins...

# 🌙 Snap Sleep: AI-Driven Sleep Airway Diagnostic Engine (iOS POC)

[![iOS](https://img.shields.io/badge/iOS-17.0+-blue.svg)](https://developer.apple.com/ios/)
[![SwiftUI](https://img.shields.io/badge/SwiftUI-Native-orange.svg)](https://developer.apple.com/xcode/swiftui/)
[![CoreML](https://img.shields.io/badge/CoreML-Edge%20AI-green.svg)](https://developer.apple.com/documentation/coreml)
[![Privacy First](https://img.shields.io/badge/Privacy-100%25%20Local-success.svg)](#)

> **Snap Sleep** 是一個建立在「邊緣運算 (Edge AI)」與「精準解剖學」之上的睡眠呼吸道診斷生態系。我們透過軟體診斷成因 (The "Why")，並提供專屬的專利硬體套組 (The "What")，徹底打破傳統止鼾器市場「盲盒式購買」的高退貨率痛點。

---

## 🚀 專案願景 (The Vision)
傳統的止鼾設備（如 TSD、MAD 或口條貼）往往未能對症下藥。Snap Sleep 採用 **Hardware-Enabled SaaS** 商業模式：
1. **先診斷 (Diagnose)：** 透過 iPhone 或外部攝影機與麥克風，在本地端捕捉睡眠時的解剖學特徵（如：下顎張開角度、喘鳴分貝）。
2. **精準給藥 (Prescribe)：** AI 引擎交叉比對出打呼的根本原因（鼻塞型、舌根塌陷、軟顎撲動、口呼吸喘鳴）。
3. **交叉銷售 (Cross-sell)：** 向使用者推薦對應的專屬硬體組合（例如：Snap Sleep 獨家專利 `X-Wing` 矽膠雙翼止鼾器、夜視攝影機）。

Phase 1 (Current): Local Edge AI via iPhone Vision & Audio Frameworks + 3D-Printed MVP.
Phase 2 (Scaling): Cloud-computing integration for deep pattern analysis & continuous model training via user feedback loops.
Phase 3 (Ecosystem): Dedicated Night Vision integration and proprietary IoT sleep peripherals.

---

## 🛡️ 隱私絕對優先 (100% Privacy-First)
本專案堅持 **「影片絕不上傳雲端」** 的最高隱私標準。
所有的影像與聲音特徵提取均透過 Apple 內建硬體神經網路引擎 (Neural Engine) 在 **手機本地端 (Local-Device)** 完成即時運算，分析完畢後自動銷毀影片快取，僅保留輕量級的 JSON 診斷日誌。

---

## 🏗️ POC 核心技術架構 (System Architecture)

### 1. 視覺特徵引擎：Visual Jaw Drop Angle (Vision Framework)
利用 iOS `Vision` 框架與 `VNDetectFaceLandmarksRequest`，在低光源環境下追蹤面部動態。
* **核心邏輯：** 即時計算上唇 (Upper Lip) 與下唇 (Lower Lip) 的 Y 軸座標距離。
* **觸發條件：** 當距離大於動態閾值且持續超過設定時間，標記為「張嘴 / 下顎後掉 (Jaw Drop)」事件。

### 2. 聲學特徵引擎：Audio dB Monitor (AVFoundation)
精準捕捉氣流受阻時產生的聲學特徵，與影像時間軸完美對齊。
* **核心邏輯：** 使用 `AVAudioRecorder` 開啟監聽 (`isMeteringEnabled = true`)。
* **資料處理：** 每秒讀取 `averagePower(forChannel: 0)` 並轉換為人類可讀的分貝值 (dB)。

### 3. 本地端診斷大腦：The 5W Cross-Reference Engine
將擷取到的資料轉化為結構化的 `5W (What, When, Why, Where, Who)` 醫療日誌：

| 醫學解剖成因 (The "Why") | AI 診斷邏輯 (The Logic) | 推薦解決方案 (The Hardware) |
| :--- | :--- | :--- |
| **口呼吸喘鳴 (Mouth Wheezing)** | `Jaw Drop 角度極大` + `連續乾澀氣流聲` | **X-Wing 矽膠雙翼** (物理限制口部亂流) |
| **舌根塌陷 (Tongue-Based)** | `嘴唇閉合或微張` + `突發性阻塞聲 / 窒息感` | **X-Wing 內部吸氣球** (舌頭穩定牽引) |
| **軟顎撲動 (Palatal Snoring)**| `下顎微閉` + `連續低頻轟隆聲 (dB 飆高)` | **X-Wing 基礎套組** (改變口腔張力) |
| **鼻部阻塞 (Nasal Snoring)** | `Jaw Drop = 0 (嘴唇緊閉)` + `高頻悶哼聲` | **鼻腔擴張貼片 (Nasal Dilator)** |

---

## 📱 核心功能展示 (Features)

### 💡 互動式診斷漏斗 (The Diagnostic Funnel)
在使用者進入睡眠監測前，App 內建基於 D3.js / SwiftUI 的 **人體呼吸道剖面模擬器**。
透過視覺化氣流動力學與「物理衝突點」，教育使用者打呼成因，並建立 AI 模型的基準線 (Baseline)。

### 📊 睡眠日誌分析 (Sleep Report)
早晨醒來時，產出精美的本地端儀表板，明確指出昨晚發生了幾次「下顎後掉」與「氣道阻塞」，並順暢引導至 Snap Sleep 專屬硬體的購買頁面。

---

## 🗺️ 產品發展路線圖 (Roadmap)

* [x] **Phase 0:** 硬體 MVP (Bambu Lab 3D 列印) 與市場競品物理衝突分析。
* [x] **Phase 1 (Current):** iOS 原生 App POC，驗證 Edge AI 捕捉 Jaw Drop Angle 的可行性。
* [ ] **Phase 2:** 軟硬體整合測試，透過 App 漏斗開始發售 `X-Wing` 止鼾套組。
* [ ] **Phase 3 (Future):** 推出帶有醫療級紅外線的「Snap Sleep 專屬睡眠雷達 (IP Camera)」，向高階用戶進行升級銷售 (Upsell)。

---

## 🔒 關於開源與智財權 (About Open Source & IP)
本 repository 為 **櫥窗展示版 (Showcase)**，旨在展示團隊架構能力與技術願景。
為保護 Snap Sleep 的核心演算法、CoreML 權重以及 X-Wing 的物理參數設計，核心商業邏輯部分以閉源方式維護。針對 UI 元件與基礎擴充套件，我們將逐步抽離並開源回饋社群。

*Designed with 🌙 by the Snap Sleep Team.*
