# ezBarControl

> 一個不需要螢幕錄製權限的 macOS 選單列管理工具
> A privacy-respecting menu bar manager for macOS — without Screen Recording

<!-- 這裡放主視覺截圖 / Place hero screenshot here -->
<!-- ![ezBarControl 主面板](docs/screenshots/hero.png) -->

## 📥 下載 / Download

**最新版本 / Latest:** [**ezBarControl 1.0**](https://github.com/Adam1313943/ezBarControl-public/releases/latest)

直接下載 DMG / Direct DMG download:
[**ezBarControl-1.0.dmg**](https://github.com/Adam1313943/ezBarControl-public/releases/download/v1.0/ezBarControl-1.0.dmg)
(858 KB · macOS 26+ · Universal Binary)

完整版本歷史請見 [Releases](https://github.com/Adam1313943/ezBarControl-public/releases) 與 [CHANGELOG.md](CHANGELOG.md)。

---

[English](#english) | [中文（繁體）](#中文繁體)

---

## 中文（繁體）

### 為什麼做這個？

Bartender 5 從 macOS Sonoma 開始要求**螢幕錄製權限**才能辨識選單列圖示。對日常使用者來說，把整個螢幕的內容（包含密碼、訊息、信用卡）授權給一個選單列工具實在不划算。

ezBarControl **只用 macOS 公開的 Accessibility API**，做到絕大多數同類工具的核心功能：

- 🔍 **快速搜尋啟動** — `⌃ Space` 叫出所有選單列圖示，含被瀏海／App menu 擋住的
- 🔄 **拖曳重排** — 直接在面板裡拖曳重新排序（對支援 reorder 的圖示會自動透過 ⌘-drag 套用）
- 👁️ **看見被擋住的圖示** — 即使在小螢幕、長 App menu 的情境，也能操作那些藏起來的圖示
- 🪶 **不需要 Screen Recording 權限**
- 🔐 **完全離線** — 不收集資料、不連網、不寫雲端日誌

### 系統需求

- macOS **26（Tahoe）或以上**
- Apple Silicon 或 Intel Mac
- 需要授予 **Accessibility 權限**（不需要 Screen Recording）

### 安裝

1. 從 [Releases](https://github.com/Adam1313943/ezBarControl-public/releases) 下載最新版 `ezBarControl-X.Y.Z.dmg`
2. 雙擊掛載 DMG，把 `ezBarControl.app` 拖進 `/Applications` 資料夾
3. 退出 DMG（或拖到垃圾桶卸載）
4. 第一次啟動：**系統設定 → 隱私權與安全性 → 輔助使用 → 加入 ezBarControl**
5. 重啟 App

> 因為本 App 經 Apple 公證（Notarized），雙擊就會打開，不會跳「無法驗證的開發者」警告。

### 使用

按 **`⌃ Space`** 叫出主面板（hotkey 可在設定裡改）。

| 動作 | 操作 |
|---|---|
| 打開／關閉面板 | `⌃ Space`（預設） |
| 搜尋圖示 | 直接打字 |
| 重排圖示 | 在列表上拖曳對應的列 |
| 觸發圖示 | 點該列的「觸發」按鈕 |
| 結束 App | 面板裡按右上電源鈕 / `⌘Q` |
| 關閉面板 | `ESC` |

### 已知限制

| 限制 | 原因 |
|---|---|
| 不能「真的隱藏」圖示 | macOS Sonoma 之後 Apple 把跨 process 寫入 ControlCenter 視窗鎖死，純靠公開 API 做不到 |

### 隱私

ezBarControl **完全在你的 Mac 本機運作**：

- ❌ 不收集任何使用資料
- ❌ 不發送任何網路請求
- ❌ 不使用第三方分析服務
- ❌ 不寫日誌到雲端
- ✅ 設定（hotkey）只存在你本機 `UserDefaults`

詳見 [PRIVACY.md](PRIVACY.md)。

### 授權

Proprietary。免費供個人使用，不可重新散佈或反組譯。詳見 [LICENSE.md](LICENSE.md)。

問題回報請使用 [GitHub Issues](https://github.com/Adam1313943/ezBarControl-public/issues)。

---

## English

### Why this exists

Starting with Bartender 5, the popular Mac menu bar utility began requiring **Screen Recording permission** on macOS Sonoma+ to detect menu bar icons. Granting "see everything on your screen" — including passwords, messages, and credit cards — to a tray utility feels disproportionate.

ezBarControl uses **only Apple's public Accessibility API** to deliver the same core functionality:

- 🔍 **Quick search & launch** — `⌃ Space` opens a Spotlight-style palette of every menu bar icon, including ones hidden behind the notch
- 🔄 **Drag to reorder** — Drag rows to rearrange icons (supported icons get repositioned via simulated ⌘-drag)
- 👁️ **See the hidden ones** — Even on smaller screens or with long app menus, you can still trigger icons hidden behind the notch
- 🪶 **No Screen Recording required**
- 🔐 **Fully offline** — Zero data collection, zero network, zero cloud logging

### Requirements

- macOS **26 (Tahoe) or later**
- Apple Silicon or Intel Mac
- **Accessibility permission** (Screen Recording is *not* required)

### Install

1. Download `ezBarControl-X.Y.Z.dmg` from [Releases](https://github.com/Adam1313943/ezBarControl-public/releases)
2. Double-click to mount, drag `ezBarControl.app` into `/Applications`
3. Eject the DMG (drag it to the Trash)
4. On first launch: **System Settings → Privacy & Security → Accessibility → add ezBarControl**
5. Re-launch the app

> The app is Apple Notarized; you should *not* see the "unidentified developer" warning.

### Usage

Press **`⌃ Space`** to open the palette (hotkey is configurable in Settings).

| Action | How |
|---|---|
| Toggle palette | `⌃ Space` (default) |
| Search icons | Just start typing |
| Reorder | Drag rows in the list |
| Trigger | Click the row's "Trigger" button |
| Quit | Power button in palette / `⌘Q` |
| Close palette | `ESC` |

### Known limitations

| Limitation | Reason |
|---|---|
| Can't truly *hide* icons | Since macOS Sonoma, cross-process writes to ControlCenter windows are silently rejected; impossible without private APIs |

### Privacy

ezBarControl operates **entirely on your Mac, locally**. No data collection, no network requests, no third-party services. See [PRIVACY.md](PRIVACY.md).

### License

Proprietary. Free for personal use; redistribution and reverse engineering are not permitted. See [LICENSE.md](LICENSE.md).

Issues and questions: [GitHub Issues](https://github.com/Adam1313943/ezBarControl-public/issues).
