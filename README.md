# Partner Marquee

CryptoTradersClub 合作團隊 logo 集合，給 sentiment lens 跑馬燈用。

## 結構

- `partners.json` — 合作團隊清單（名稱、圖片檔名、顯示順序）
- `*.png` / `*.jpg` — 各團隊 logo

## 新增合作團隊

1. 把新 logo 放進 repo 根目錄（建議 600px 寬以內、檔案 < 500KB）
2. 在 `partners.json` 加一筆 `{ "name": "...", "image": "..." }`
3. commit + push,前端會在下次重新整理時自動抓到

## Logo 規格

- 建議比例:橫式長條 / 正方形,前端會自動裁切高度 40px (桌面) 或 32px (手機)
- 透明背景 PNG 顯示效果最好
- 太大的圖片建議先用 tinypng.com 之類壓縮

## 前端整合

前端從 `https://raw.githubusercontent.com/HarmonicLover/partner-marquee/main/partners.json` 抓 JSON
跑馬燈會無限橫向滾動,滑鼠 hover 暫停。
  

