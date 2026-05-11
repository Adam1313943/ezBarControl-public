# ezBarControl 隱私政策 / Privacy Policy

最後更新 / Last updated: 2026-05-08

---

## 中文（繁體）

### 一句話總結

**ezBarControl 不收集、不傳送、不儲存您的任何個人資料。所有資料都只留在您的 Mac 本機。**

### 我們不做的事

| 項目 | 狀態 |
|---|---|
| 收集使用統計（analytics） | ❌ **沒有** |
| 發送網路請求 | ❌ **沒有** |
| 連接任何遠端伺服器 | ❌ **沒有** |
| 使用第三方 SDK / 追蹤工具 | ❌ **沒有** |
| 寫日誌到雲端 | ❌ **沒有** |
| 自動更新檢查（除非您手動執行） | ❌ **目前沒有** |

ezBarControl 是一個純粹的本機工具，**沒有任何網路通訊功能**。

### 本軟體取用的權限

#### Accessibility（輔助使用）權限 — 必須

**用途：** 列舉選單列上的圖示位置，以及模擬鍵盤、滑鼠事件來重排或觸發圖示。

**處理方式：** 所有讀取到的資料（圖示位置、所屬 App 名稱、AX 標題等）**只在記憶體中處理，立即用完即棄**，不會寫入任何檔案、不會送出任何網路請求。

**您可以隨時撤銷：** 系統設定 → 隱私權與安全性 → 輔助使用 → 取消勾選 ezBarControl。

#### Screen Recording（螢幕錄製）權限 — 不需要

ezBarControl **不請求**也**不需要**螢幕錄製權限。這是本軟體與 Bartender 5+ 等同類工具的主要差異點。

### 本軟體儲存的資料

僅儲存使用者偏好設定（目前為「自訂 hotkey」），存放於：

```
~/Library/Preferences/com.harmonation.ezBarControl.plist
```

這個檔案由 macOS 的 `UserDefaults` 系統管理，**僅存在您本機**，不會被同步到任何雲端服務（除非您自己用 iCloud Drive 同步整個 `~/Library`，但 macOS 預設不會這樣做）。

### 第三方服務

本軟體**不使用任何第三方服務**，包含但不限於：

- ❌ 無 Google Analytics、Firebase、Amplitude、Mixpanel 等分析服務
- ❌ 無 Sentry、Crashlytics、Bugsnag 等錯誤回報服務
- ❌ 無 Sparkle、AppCenter 等自動更新服務
- ❌ 無廣告 SDK
- ❌ 無社群登入 / 雲端同步

### 兒童隱私

本軟體並非針對 13 歲以下兒童設計，且不會主動向兒童收集任何個人資料。

### 政策變更

若未來政策有變更（例如增加自動更新功能而需要連網），本檔案將更新並標明日期。建議您在更新軟體時順便檢視本政策。

### 聯絡方式

[GitHub Issues](https://github.com/Adam1313943/ezBarControl/issues) 提交問題。

---

## English

### TL;DR

**ezBarControl collects, transmits, and stores no personal data. Everything stays on your Mac.**

### What we don't do

| Item | Status |
|---|---|
| Usage analytics | ❌ **None** |
| Network requests | ❌ **None** |
| Connection to any remote server | ❌ **None** |
| Third-party SDKs / tracking | ❌ **None** |
| Cloud logging | ❌ **None** |
| Automatic update checks (unless manually triggered) | ❌ **None at present** |

ezBarControl is a purely local utility with **no networking functionality whatsoever**.

### Permissions used

#### Accessibility — required

**Purpose:** Enumerate menu bar icon positions and simulate keyboard/mouse events to reorder or trigger them.

**How it's handled:** Any data read (icon positions, owning app names, AX titles) is **processed in memory and discarded immediately** — never written to disk, never sent over the network.

**Revoke any time:** System Settings → Privacy & Security → Accessibility → uncheck ezBarControl.

#### Screen Recording — not required

ezBarControl **does not request** and **does not need** Screen Recording permission. This is the primary differentiator from Bartender 5+ and similar utilities.

### What we store

Only your user preferences (currently just the custom hotkey), stored at:

```
~/Library/Preferences/com.harmonation.ezBarControl.plist
```

This file is managed by macOS's `UserDefaults` system, exists **only on your local Mac**, and is not synced to any cloud service (unless you've manually configured iCloud Drive to sync `~/Library`, which macOS doesn't do by default).

### Third-party services

This software **uses no third-party services**, including but not limited to:

- ❌ No Google Analytics, Firebase, Amplitude, Mixpanel, etc.
- ❌ No Sentry, Crashlytics, Bugsnag, etc.
- ❌ No Sparkle, AppCenter, or other auto-update services
- ❌ No advertising SDKs
- ❌ No social login / cloud sync

### Children's privacy

This software is not designed for children under 13, and we do not knowingly collect personal information from children.

### Policy changes

If this policy changes in the future (e.g., adding an auto-update feature that requires network access), this document will be updated with a new date. We recommend reviewing this policy when updating the software.

### Contact

Please file [GitHub Issues](https://github.com/Adam1313943/ezBarControl/issues) for questions.

---

© 2026 CHING FENG WANG / Harmonation
