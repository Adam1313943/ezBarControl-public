# Changelog

本檔案紀錄 ezBarControl 各版本的變更。
All notable changes to ezBarControl are documented here.

格式參考 [Keep a Changelog](https://keepachangelog.com/zh-TW/1.1.0/)。
版本號採用 [Semantic Versioning](https://semver.org/lang/zh-TW/)。

---

## [Unreleased]

待發佈中。

---

## [1.0] - 2026-05-11

首版公開發佈 / Initial public release.

### 新增 / Added
- 全域快捷鍵 `⌃ Space` 開啟主面板（可在設定中變更）
- 自動偵測選單列上所有圖示，包含被瀏海／App menu 擋住的
- 拖曳列表項目重新排序（對支援 reorder 的圖示自動透過模擬 ⌘-drag 套用）
- 「Pull with rotations」演算法：把藏在右側的圖示透過反向推擠拉到可視區
- 點擊「觸發」按鈕直接打開圖示選單（AXPress 為主、CGEvent 模擬點擊為備援）
- 啟動時自動開啟面板，方便首次使用
- SwiftUI 設定面板：可自訂 hotkey
- .app 經 Apple Notarization，雙擊即可開啟

### 校驗碼 / Checksum
- `ezBarControl-1.0.dmg`：`15197ef148498fe05ccbd11d95eff8a14084fb1962ceed5468160f491dc3d2eb`

### 已知限制 / Known limitations
- OneDrive 圖示無法重排（Microsoft 沒在它的 `NSStatusItem` 開啟 reorder behavior）
- pCloud 圖示無法被 Accessibility API 偵測
- 不支援「真正隱藏圖示」（macOS Sonoma+ 鎖死了跨 process 視窗寫入）

### 系統需求 / Requirements
- macOS 26 (Tahoe) 或以上
- Accessibility 權限
