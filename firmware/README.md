# 時鐘更新目錄

時鐘讀取 main 分支此目錄的 `latest.json`，比對已簽章的版本資訊，再從清單中的下載位址取得 Releases 韌體。

按時鐘「設定 → 韌體更新 → 檢查更新」即可檢查。有新版時按「下載並更新」。公開目錄不需在裝置登入 GitHub。

發布新版時，先將 bin 和已簽章 manifest 發布到 Releases，再用本機專案 scripts/publish_ota_feed.py 同步此目錄的 latest.json。腳本會先驗證簽章與發布檔，才更新清單。

請使用本機打包工具產生的清單；手動修改 payload 會使簽章失效。上傳任意 bin 或原始碼不會自動產生可用更新。不要上傳 Wi-Fi 密碼、裝置備份或簽章私鑰。
