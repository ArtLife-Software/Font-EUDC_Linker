# Font-EUDC Linker

![OS](https://img.shields.io/badge/OS-Windows-blue?style=flat-square&logo=windows)
![Language](https://img.shields.io/badge/Language-AutoHotkey_v2-green?style=flat-square&logo=autohotkey)
![Locale](https://img.shields.io/badge/Locale-正體中文-orange?style=flat-square)
![License](https://img.shields.io/badge/License-GPL_v3-red?style=flat-square)
![Latest Release](https://img.shields.io/github/v/release/ArtLife-Software/Font-EUDC_Linker?style=flat-square&color=blue)
![Downloads](https://img.shields.io/github/downloads/ArtLife-Software/Font-EUDCLinker/total?style=flat-square&logo=github)

**Font-EUDC Linker** 是一款專為 Windows 環境設計的造字關聯管理工具。透過直覺的圖形介面，協助使用者快速建立、維護及批次部署字型與造字檔（`.tte`）之間的關聯。

---

## 核心功能

* **雙軌制管理**：支援同時管理 **目前使用者 (HKCU)** 與 **全部使用者 (HKLM)** 的造字設定。
* **自動化掃描**：一鍵掃描系統內所有已安裝字型，並即時呈現目前的造字關聯路徑。
* **精準清理**：智慧偵測無效的關聯（如字型已刪除或 `.tte` 檔案已移動），保持登錄檔（Registry）乾淨。
* **批次部署**：可匯出自動化批次檔（`.bat`），方便在多台電腦上快速部署相同的造字環境。
* **防呆機制**：內建自動提權邏輯與 UI 互鎖保護，確保關鍵操作擁有足夠權限並降低誤觸風險。

---

## 使用環境

* **作業系統**：Windows 10 / 11 (x64)
* **權限需求**：由於涉及 HKLM 登錄檔操作，程式執行時會要求 **系統管理員權限**。
* **開發語言**：AutoHotkey v2.0+

---

## 安裝與使用

### 1. 執行程式
下載編譯後的執行檔或透過 AutoHotkey v2 執行腳本。啟動時若未具備管理員權限，程式將自動提示提權。

### 2. 管理造字檔
* 點擊 **「新增造字檔」** 將您的 `.tte` 檔案加入左側清單。
* 程式會記憶您的歷史清單，方便下次快速選取。

### 3. 建立關聯
1.  從左側選中一個 **造字檔**。
2.  從右側選中一個或多個（支援 `Ctrl` / `Shift` 複選） **字型**。
3.  勾選欲套用的範圍（個人或全域）。
4.  點擊 **「執行關聯」** 即可完成部署。

---

## 專案資訊

* **設計開發**：林彥丞 (Lin Yancheng)
* **品牌標誌**：[ArtLife Software](https://github.com/ArtLife-Software)
* **授權協議**：GPL-3.0 License
* **聯繫信箱**：lin.yancheng@outlook.com

---

## 社群連結

如果您有任何問題或建議，歡迎透過以下管道參與討論：
* **GitHub Issues**：回報 Bug 或提出功能需求。
* **Facebook 社團**：[O & C VBA 研究社](https://www.facebook.com/groups/vba.club)

---

### 免責聲明
本工具會修改系統登錄檔（Registry），雖然內建防呆機制，但在大規模部署前仍建議先行備份相關機碼。對於因操作不當導致的系統問題，開發者不負損害賠償責任。
