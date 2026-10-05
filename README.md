# 𓃥 白六 3D GLB 骨牌互動模擬器 (Dominoes Message)

一個基於 **Three.js** 與 **WebGL** 開發的 3D 手繪骨牌互動網頁應用程式。支援自由手繪骨牌軌道、動態 3D 陸橋爬升、霓虹文字陣列與骨牌推倒觸發特效，並提供即時運鏡追蹤與 WebM 視訊錄影功能。

👉 **線上展示 (Live Demo)**：[https://kuochili-ops.github.io/Dominoes-message/](https://kuochili-ops.github.io/Dominoes-message/)

---

## ✨ 核心特色 (Features)

* 🎨 **2D 正交手繪與 3D 自由視角 (2D/3D Mode Switch)**
  * **畫線模式**：採用正交俯視角，方便精準繪製骨牌路線與佈置文字區塊。
  * **視角模式**：切換為 3D 透視鏡頭，支援全方位旋轉、平移與縮放視角。

* 🌉 **智慧兩點式陸橋演算 (Smart 3D Arch Bridge)**
  * **雙點快速建置**：點擊第一點（起點）與第二點（過橋頂點），系統會自動計算合理的骨牌爬升與下降軌道。
  * **手動微調控制球**：生成後可自由拖曳紅色控制球精準調整坡度範圍。
  * **自動隱藏標記**：切換至 3D 觀察模式時，自動隱藏陸橋控制球，呈現乾淨逼真的立體軌道。

* 🀄 **動態 3D 骨牌與自訂樣式 (Customizable Dominoes)**
  * 支援載入外部 `.glb` 3D 骨牌模型，並隨時調整骨牌尺寸比例與排列間距。
  * 提供骨牌與霓虹文字區塊的即時自訂色彩選擇器。

* 🎆 **霓虹文字區塊與煙火特效 (Neon Text & Fireworks Effect)**
  * 可自由新增中文/英文文字區塊，支援 2D 平面拖曳與四角等比例縮放。
  * 骨牌倒下並碰觸到文字區塊時，會觸發字體升起顯示與多色粒子煙火綻放特效。

* 📹 **鏡頭追蹤與高畫質錄影 (Camera Tracking & Screen Recording)**
  * **動態追蹤攝影**：骨牌推倒時，鏡頭自動順暢跟隨最前方的倒下骨牌。
  * **一鍵視訊錄影**：內建 WebM 格式錄影功能，推倒完成後自動下載高畫質影片。

---

## 🛠️ 技術架構 (Tech Stack)

* **Core Engine**: HTML5 / JavaScript (ES6+)
* **3D Rendering**: [Three.js](https://threejs.org/) (r128)
* **3D Model Loader**: `GLTFLoader` (載入 `.glb` 骨牌模型)
* **Physics & Math**: Catmull-Rom 曲線路徑插值、自訂骨牌連鎖碰撞邏輯與物理傾倒計算
* **Deployment**: GitHub Pages

---

## 🚀 快速開始 (Quick Start)

本專案為純前端應用，不需要複雜的建置環境或 Node.js 依賴：

1. **複製專案 (Clone Repository)**
   ```bash
   git clone [https://github.com/kuochili-ops/Dominoes-message.git](https://github.com/kuochili-ops/Dominoes-message.git)
   cd Dominoes-message
