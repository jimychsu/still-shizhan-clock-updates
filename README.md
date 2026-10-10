# STILL 實戰派桌上時鐘更新

適用立創實戰派 ESP32-S3、320×240 ST7789。此儲存庫提供已簽章的韌體更新，不適用 Waveshare 七吋板。

在已安裝 OTA 功能的時鐘上連接 Wi-Fi，進入「設定 → 韌體更新 → 檢查更新」，有新版時選「下載並更新」。

更新來源：https://raw.githubusercontent.com/jimychsu/still-shizhan-clock-updates/main/firmware/latest.json

每個 Release 提供應用程式 bin、RSA 簽章版本資訊 latest.json 與 SHA256SUMS.txt。首次安裝需 USB 及相符的分割表；不要把應用程式 bin 當成完整 Flash 映像。

Wi-Fi 密碼儲存在裝置，不包含於發布檔。簽章私鑰不公開。
