# 酒類電商網站 wineshop-platform

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Material Icons](https://img.shields.io/badge/Material_Icons-757575?style=for-the-badge&logo=google&logoColor=white)](https://fonts.google.com/icons)
[![License](https://img.shields.io/badge/License-Personal_Use-blue?style=for-the-badge)](#版權聲明)

## 專案簡介

這是一個為「新酒節限時 72 小時」活動設計的完整電商網頁，整合了真實商品圖片與現代化的 UI 設計。專案採用純前端技術實現，無需後端即可展示完整的電商頁面效果。

## 網址

[wineshop-platform.vercel.app](https://wineshop-platform.vercel.app/)

## 核心價值

- **真實圖片素材**：使用實際商品圖片提升視覺真實感
- **Material Design Icons**：Google Material Icons 提供專業圖示系統
- **完整 RWD 設計**：三種裝置尺寸完美適配
- **純前端實現**：無需後端，開箱即用
- **豐富互動效果**：Hover、動畫、即時回饋

## 技術架構

### 核心技術
```
├── HTML5
│   ├── 語意化標籤（header, nav, main, section, footer）
│   └── SEO 優化結構
├── CSS3
│   ├── Flexbox 彈性佈局
│   ├── Grid 網格系統
│   ├── CSS Variables（顏色系統）
│   ├── Transform & Transition 動畫
│   ├── Filter 濾鏡效果
│   └── Backdrop-filter 毛玻璃效果
└── JavaScript (Vanilla)
    ├── DOM 操作與事件監聽
    ├── 倒數計時功能
    ├── 平滑捲動效果
    └── 互動動畫控制
```

### 外部資源
- **Google Material Icons**
  ```html
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
  ```
- **Google Fonts (Noto Sans TC)**
  - 預設字體家族：`'Noto Sans TC', -apple-system, sans-serif`

## 專案結構

```
wineshop-platform/
│
├── index.html             # 主頁面（Single Page Application）
├── README.md              # 專案說明文件
│
└── assets/                # 圖片資源目錄 必要
    ├── hero.jpg           # Hero Banner 背景圖
    ├── edm-header.jpg     # EDM 首屏背景圖
    ├── product1.jpg       # 商品 1：法國波爾多紅酒雙瓶組
    ├── product2.jpg       # 商品 2：義大利經典氣泡酒
    ├── product3.jpg       # 商品 3：西班牙珍藏陳年紅酒
    └── product4.jpg       # 商品 4：蘇格蘭單一麥芽威士忌
```

## 安裝與啟動

### 前置需求
- 現代瀏覽器（Chrome 90+, Firefox 88+, Safari 14+）
- 圖片素材（參考上方「圖片檔案要求」）
- 基本的 HTML/CSS 知識

### 安裝步驟

#### 方法一：直接下載

1. **下載專案**
   ```bash
   # 下載 ZIP 或 Clone 專案
   git clone https://github.com/tinachen0326/wineshop-platform.git
   cd wineshop-platform
   ```

2. **準備圖片資源**
   ```bash
   # 建立 assets 資料夾
   mkdir assets
   
   # 將 6 張圖片放入 assets 資料夾
   # hero.jpg, edm-header.jpg, product1-4.jpg
   ```

3. **開啟網頁**
   ```bash
   # 方式 1: 直接開啟
   open index.html
   
   # 方式 2: VS Code Live Server
   # 右鍵 index.html → Open with Live Server
   
   # 方式 3: Python 簡易伺服器
   python -m http.server 8000
   # 瀏覽器開啟 http://localhost:8000
   
   # 方式 4: Node.js http-server
   npx http-server -p 8000
   ```

#### 方法二：線上編輯

1. 使用 [CodePen](https://codepen.io/) 或 [JSFiddle](https://jsfiddle.net/)
2. 將 HTML 貼入編輯器
3. 圖片使用線上圖床（如 Imgur、Unsplash）

## 瀏覽器支援

### 完整支援

| 瀏覽器 | 版本 | 說明 |
|--------|------|------|
| Chrome |  90+ | 完整支援所有功能 |
| Firefox |  88+ | 完整支援所有功能 |
| Safari |  14+ | 完整支援所有功能 |
| Edge |  90+ | 完整支援所有功能 |
| Opera |  76+ | 完整支援所有功能 |

### 部分支援

| 瀏覽器 | 版本 | 說明 |
|--------|------|------|
| Safari |  13 | backdrop-filter 需要加前綴 |
| iOS Safari |  13+ | 部分毛玻璃效果可能不顯示 |

### 不支援

| 瀏覽器 | 說明 |
|--------|------|
| IE 11 |  不支援 CSS Grid, Flexbox gap |
| IE 10 及以下 |  完全不支援 |

### 功能相容性

```
 CSS Grid Layout          (所有現代瀏覽器)
 Flexbox                  (所有現代瀏覽器)
 CSS Transform/Transition (所有現代瀏覽器)
 Filter 濾鏡　　　　　　　　(所有現代瀏覽器)              
 Backdrop-filter   　　　　(Safari 需要 -webkit- 前綴) 　  　
 object-fit　　　　　　　　(所有現代瀏覽器)
 ES6 JavaScript         　(所有現代瀏覽器)
```

## 注意事項

### 1. 圖片資源

**必須準備圖片檔案**
```
 錯誤：沒有準備圖片 → 頁面顯示空白或破圖
 正確：準備 6 張圖片放入 assets/ 資料夾
```

**圖片命名規則**
- 嚴格遵循檔名：`hero.jpg`, `edm-header.jpg`, `product1.jpg` 等
- 大小寫敏感（Linux/Mac）
- 不可使用空格或特殊字元

### 2. Material Icons

**需要網路連線**
```html
<!-- 此行需要網路載入 -->
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
```

**離線使用方案：**
1. 下載 Material Icons 字體檔
2. 自行託管（self-hosted）
3. 或改用 SVG 圖示

### ３. 效能考量

**圖片優化建議**
```
- 使用 WebP 格式（更小的檔案大小）
- 壓縮圖片（TinyPNG、ImageOptim）
- 設定適當的尺寸（避免載入過大圖片）
- 考慮使用 lazy loading
```

## 致謝

### 設計靈感
- 參考現代電商網站設計趨勢
- Material Design 設計語言

### 技術資源
- [Google Material Icons](https://fonts.google.com/icons) - 圖示系統
- [Google Fonts](https://fonts.google.com/) - Noto Sans TC 字體
- [MDN Web Docs](https://developer.mozilla.org/) - 技術文件

### 社群支持
- 感謝所有提供回饋與建議的使用者
- 感謝所有 Contributors 的貢獻
  
**法律聲明**  
依據法律規定，未滿 18 歲者，禁止購買及飲用酒類。  
請理性飲酒，酒後不開車，安全有保障。

## 版權聲明

此專案僅供個人學習與紀錄使用，無授權任何學習教材用途與商業用途。
