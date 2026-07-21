# Snap Sleep
Where the SLEEP begins...

# 🌙 Snap Sleep: 自我進化的多模態 AI 睡眠代理 (Self-Evolving AI Sleep Agent)

[![Agent-Native](https://img.shields.io/badge/Architecture-Agent--Native-red.svg)](#)
[![Multi-Modal AI](https://img.shields.io/badge/AI-Multi--Modal-purple.svg)](#)
[![Edge to Cloud](https://img.shields.io/badge/Scale-Edge_to_Cloud-blue.svg)](#)
[![iOS](https://img.shields.io/badge/iOS-Native%20Vision-blue.svg)](https://developer.apple.com/ios/)

> **Snap Sleep** 是一個代理原生 (Agent-Native)、具備隱私保護且能自我進化的睡眠健康生態系。我們將多模態 AI（影像與聲學）轉化為感測基礎設施，讓 AI 代理不僅能「診斷」打呼的機械性成因，更能主動「介入」提供客製化硬體處方（X-Wing 模組），並根據使用者的真實反饋進行模型優化，創造一個持續進步的物理健康閉環 (Physical-Digital Recovery Loop)。

---

## 🚀 專案願景：代理原生時代的睡眠基礎設施
傳統的睡眠 App 只是被動顯示數據的儀表板。Snap Sleep 是一個**主動式 AI 健康代理 (Autonomous Health Agent)**。
1. **感知 (Sense - 多模態基礎設施)：** 利用邊緣運算（初期透過 iPhone，未來擴展至專屬夜視攝影機）在低光源下捕捉面部生物力學與氣流聲學特徵。
2. **診斷 (Diagnose)：** AI 引擎精準判斷打呼的物理根源（下顎後掉、舌根塌陷、軟顎撲動）。
3. **介入 (Intervene)：** 代理會開立專屬的物理干擾處方——我們獨家專利、可快速 3D 列印成型的 `X-Wing` 矽膠干擾機制。
4. **進化 (Evolve)：** 透過測量隔夜的生物數據變化與使用者的主觀反饋，AI 代理會自我訓練並持續優化其診斷與治療模型。

---

## 🛡️ 隱私絕對優先與數據擴展 (Privacy-First & Scalable)
在 POC 階段，我們堅持 **「影片絕不上傳雲端」**。
所有的影像提取均透過 Apple 內建硬體神經網路引擎 (Neural Engine) 在 **手機本地端 (Edge AI)** 完成即時運算。隨著系統擴展，我們僅上傳去識別化的數值標籤（如：時間軸、角度偏移值、分貝參數）至雲端進行深度模型訓練，確保最高隱私標準的同時，賦予 AI 自我進化的能力。

---

## 🏗️ 核心技術架構 (System Architecture)

### 1. 多模態感知引擎 (Multi-Modal Sensory Infrastructure)
* **視覺特徵引擎 (Vision Framework)：** 利用 `VNDetectFaceLandmarksRequest` 在低光源下追蹤動態。即時計算上/下唇的 Y 軸座標距離，精準捕捉「張嘴 / 下顎後掉 (Jaw Drop)」事件。
* **聲學特徵引擎 (AVFoundation)：** 使用 `AVAudioRecorder` (`isMeteringEnabled = true`) 監聽氣流受阻的頻率與分貝 (dB) 變化，並與視覺時間軸完美對齊。

### 2. 診斷大腦與自學習迴圈 (The AI Agent Brain)
將擷取到的資料轉化為結構化的 `5W (What, When, Why, Where, Who)` 醫療日誌，並進行交叉比對：

| 醫學解剖成因 (The "Why") | 多模態 AI 診斷邏輯 (Vision + Sound) | AI 推薦介入方案 (The Hardware) |
| :--- | :--- | :--- |
| **口呼吸喘鳴 (Mouth Wheezing)** | `Jaw Drop 角度極大` + `連續乾澀氣流聲` | **X-Wing 矽膠雙翼** (物理限制口部亂流) |
| **舌根塌陷 (Tongue-Based)** | `嘴唇閉合或微張` + `突發性阻塞聲 / 窒息感` | **X-Wing 內部吸氣球** (舌頭穩定牽引) |
| **軟顎撲動 (Palatal Snoring)**| `下顎微閉` + `連續低頻轟隆聲 (dB 飆高)` | **X-Wing 基礎套組** (改變口腔張力) |
| **鼻部阻塞 (Nasal Snoring)** | `Jaw Drop = 0 (嘴唇緊閉)` + `高頻悶哼聲` | **鼻腔擴張貼片 (Nasal Dilator)** |

---

## 🗺️ 產品發展路線圖 (Roadmap)

這是一場從邊緣運算走向全生態系的革命：

* [x] **Phase 1 (Current) - Edge AI & MVP：** 基於 iOS Vision & Audio Frameworks 的本地端多模態概念驗證，結合 Bambu Lab A1 快速打樣的 X-Wing 物理干擾設備。
* [ ] **Phase 2 (Scaling) - Cloud Computing & Self-Evolving：** 整合雲端運算，進行深度模式分析。導入使用者反饋迴圈 (User Feedback Loops)，讓 AI 代理根據真實的隔夜療效，自動訓練並優化推薦模型。
* [ ] **Phase 3 (Ecosystem) - IoT & Night Vision：** 推出帶有機器視覺的「Snap Sleep 專屬夜視攝影機」與智慧睡眠周邊設備，完整涵蓋高階使用者的自我改善生態系。

---

## 🔒 關於開源與智財權 (About Open Source & IP)
本 repository 為 **櫥窗展示版 (Showcase)**，旨在向投資人與技術夥伴展示團隊的 Agent-Native 系統架構能力與技術願景。
為保護 Snap Sleep 的多模態核心演算法、自我進化權重以及 X-Wing 的物理參數設計，核心商業邏輯以閉源方式維護。針對 UI 元件、視覺化漏斗與基礎 API，我們將逐步抽離並開源回饋社群。

*Designed with 🌙 by the Snap Sleep Team. (Silicon Valley Software DNA x Taiwan Hardware Iteration)*
