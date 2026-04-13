<div align="center">

# ✨ Particle Type

**互動式粒子文字聚合展示**

輸入文字 → 粒子消散 → 重新聚合成你打的字

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://prayer168.github.io/particle_type/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)]()
[![Canvas](https://img.shields.io/badge/Canvas%20API-FF6F00?style=for-the-badge&logo=html5&logoColor=white)]()

<br />

🔗 **線上展示：https://prayer168.github.io/particle_type/**

</div>

---

## 📖 專案介紹

**Particle Type** 是一個以 HTML Canvas 製作的互動式粒子文字展示頁面。

使用者在輸入框打字後，畫面中原本自由漂浮的數千顆粒子，會先觸發消散動畫，接著帶著拖尾效果逐步重新聚合，最終排列成你輸入的文字。

這個專案特別適合作為：

- 🎨 個人作品集首頁 Hero Section
- 🏢 品牌展示頁主視覺
- 🎭 展演互動裝置頁面
- 💻 創意前端互動練習作品

---

## 🎯 功能特色

| 功能 | 說明 |
|------|------|
| 🔤 粒子聚字 | 輸入文字後，粒子會自動聚合排列成文字形狀 |
| 🌈 漸層色彩 | 粒子依據位置映射藍→紫→粉的流動漸層 |
| 💫 粒子拖尾 | 每顆粒子移動時留下柔和的光跡殘影 |
| 🖱️ 滑鼠吸附 | 滑鼠靠近時粒子會被游標吸引 |
| 💥 按住排斥 | 按住滑鼠時切換為排斥模式，粒子被推開 |
| 🎆 消散動畫 | 文字切換時粒子先炸散再重新聚合 |
| 🔄 自動輪播 | 內建自動輪播展示詞，適合無人展示場景 |
| 🌌 背景星塵 | 額外一層微弱星塵粒子緩緩飄落 |
| 🔗 粒子連線 | 靠近的粒子之間會產生淡淡的連線效果 |
| ✨ Aurora 光暈 | 背景有緩慢移動的極光色彩光暈 |
| 📱 觸控支援 | 支援手機與平板的觸控操作 |
| 🀄 多語言 | 支援中文、英文、數字 |

---

## 🕹️ 操作方式

### 鍵盤與滑鼠

| 操作 | 效果 |
|------|------|
| 輸入框打字 | 粒子消散後重新聚合成文字 |
| 滑鼠移動 | 吸附附近的粒子 |
| 按住滑鼠 | 切換為排斥模式，推開粒子 |
| `Space` 空白鍵 | 觸發全畫面爆散效果 |
| `Enter` 確認鍵 | 重新套用目前輸入的文字 |

### 按鈕控制

| 按鈕 | 功能 |
|------|------|
| **重組文字** | 重新觸發消散 → 聚合動畫 |
| **消散特效** | 讓所有粒子爆散，短暫後自動重組 |
| **自動輪播：開／關** | 切換自動輪播展示模式 |

---

## 🛠️ 技術架構

```
純前端靜態頁面，零依賴，單一 HTML 檔案
```

- **HTML5** — 頁面結構
- **CSS3** — 玻璃擬態 UI、響應式排版、Aurora 漸層背景
- **JavaScript (Vanilla)** — 粒子物理引擎、動畫迴圈、互動邏輯
- **Canvas API** — 粒子繪製、拖尾渲染、光暈效果

### 核心技術原理

1. **文字取樣**：將輸入文字繪製到隱藏的 Canvas，透過 `getImageData()` 掃描像素位置
2. **粒子系統**：每顆粒子擁有位置、速度、目標座標、色相等屬性
3. **趨近力 + 摩擦力**：粒子以物理模擬方式緩慢靠近目標，產生自然聚合感
4. **軌跡記錄**：每顆粒子保留近幾幀的歷史位置，用於繪製拖尾
5. **滑鼠互動**：計算粒子與游標距離，施加吸引力或排斥力

---

## 📂 專案結構

```bash
particle_type/
├── index.html      # 主程式（HTML + CSS + JavaScript 全包）
├── README.md       # 專案說明文件
└── .nojekyll       # 避免 GitHub Pages 進行 Jekyll 處理
```

---

## 🚀 快速開始

### 本機預覽

```bash
# 方法一：直接開啟
open index.html

# 方法二：使用 Python 簡易伺服器
python3 -m http.server 8080

# 方法三：使用 VS Code Live Server 擴充套件
# 安裝後對 index.html 按右鍵 → Open with Live Server
```

### 部署到 GitHub Pages

```bash
# 1. Clone 此專案
git clone https://github.com/prayer168/particle_type.git
cd particle_type

# 2. 進行修改後推送
git add .
git commit -m "Update particle hero"
git push origin main
```

接著到 GitHub repository：

1. 點選 **Settings**
2. 左側選單找到 **Pages**
3. **Source** 選擇 `Deploy from a branch`
4. **Branch** 選擇 `main`，資料夾選 `/ (root)`
5. 點選 **Save**
6. 等待幾分鐘後即可訪問

---

## ⚙️ 自訂參數

你可以在 `index.html` 的 `config` 物件中調整以下參數：

| 參數 | 預設值 | 說明 |
|------|--------|------|
| `baseParticles` | 自動計算 | 基礎粒子數量（依螢幕面積自動調整） |
| `maxParticles` | `3200` | 粒子數量上限 |
| `trailLength` | `12` | 拖尾長度，越大越夢幻 |
| `dissolveBurst` | `8.5` | 消散爆發力道，越大越炸裂 |
| `mouseRadius` | `180` | 滑鼠影響範圍（像素） |
| `mouseStrength` | `0.24` | 滑鼠吸附強度 |
| `repelStrength` | `0.34` | 按住時排斥強度 |
| `sampleGap` | `5` | 文字取樣間距，越小越精細 |
| `textAttract` | `0.050` | 粒子朝文字聚合的趨近力 |
| `friction` | `0.88` | 摩擦力，影響粒子減速手感 |
| `dustCount` | `120` | 背景星塵粒子數量 |

---

## 🌐 瀏覽器支援

| 瀏覽器 | 支援 |
|--------|------|
| Chrome | ✅ |
| Firefox | ✅ |
| Safari | ✅ |
| Edge | ✅ |
| 手機瀏覽器 | ✅ |

---

## 📄 License

This project is open for personal portfolio and demo use.

---

<div align="center">

Made with ❤️ by [prayer168](https://github.com/prayer168)

**⭐ 如果你喜歡這個專案，歡迎給一顆 Star！**

</div>
