# GitPeeker

換個方式，看見專案。文件、網站與影音，在同一個桌面視窗預覽，無須完整 clone 儲存庫。

## 下載

0.7 起提供下表的多平台版本；請以實際已發布附件為準。

[最新發行與各平台直接下載](https://github.com/CodingCatz/GitPeeker-Releases/releases/latest)

| 平台 | 建議格式 | 另一種格式 |
|---|---|---|
| Windows 10／11 x64 | Setup.exe 安裝版 | Portable.exe 免安裝版 |
| Mac Apple Silicon（M 系列） | macOS-arm64.dmg | macOS-arm64.zip |
| Linux x64 | Linux-x64.deb（Ubuntu 24.04） | — |

Mac 只維護 Apple Silicon，不提供 Intel 版。只下載自己的平台與 CPU 架構，不需要另外安裝 Node.js、Rust 或 Git。

Mac：DMG 打開後把 GitPeeker 拖到 Applications；ZIP 解壓後使用 GitPeeker.app。測試版尚未取得 Apple Developer ID／公證，首次開啟可能需要依 macOS「隱私權與安全性」提示允許。參閱 [Apple 官方說明](https://support.apple.com/102445)。

Linux 實測基準為 Ubuntu 24.04 x64，其他發行版尚未實測。

Linux：使用系統套件安裝器安裝 DEB，正式包保持 Chromium 沙箱開啟。請使用一般桌面帳號啟動。記住登入需要 GNOME Keyring／KWallet 等系統安全金鑰服務，不會降為明文保存。

## 更新與資料

- Windows 上方「檢查更新」可取得新版。確認後才背景下載，驗證簽章與 SHA256，正常關閉並背景重開。安裝版與免安裝版皆支援。
- Mac／Linux 本版手動換版，尚未提供程式內更新。
- 同一電腦、同一作業系統帳號下，固定應用程式身分與資料目錄讓換包／改版沿用登入及設定。請勾選「記住登入」；加密憑證不能直接搬到另一個帳號或作業系統。
- 檢查更新不需要 GitHub 登入，不消耗 GitHub REST API 額度。讀取私人儲存庫仍需本人授權。
- Windows 尚無 Authenticode 簽章；Mac 使用 ad-hoc 簽章，尚無 Apple Developer ID／公證。

## 其他下載項目

update-manifest.json／sig 是 Windows 程式讀取的更新清單與簽章。SHA256SUMS 是手動核對檔案使用。一般使用者不必下載這些檔案。

驗證報告與重啟維護腳本保留在私人來源。GitHub 自動提供的 Source code ZIP／tar.gz 只包含本公開發行庫的說明文件，不是 GitPeeker 私人原碼。

本庫只公開發行附件與說明；原碼儲存庫維持私人。

