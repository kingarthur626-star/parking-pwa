停車位收入管理系統｜PWA Static V1.2 Launcher

正確問題：
- GitHub PWA 頁面本身可以開啟。
- 原 V1.1 使用 iframe 內嵌 Apps Script，因此 Google 顯示 403。
- 點右上角「開啟」後，改成直接開 Apps Script，所以正式系統正常。

V1.2 修正：
1. 完全移除 iframe。
2. 從主畫面啟動後，直接以頂層頁面開啟正式 Apps Script。
3. 新增網站根目錄 apple-touch-icon.png（180×180、無透明背景）。
4. 同時加入 apple-touch-icon 與 apple-touch-icon-precomposed。
5. 更新 manifest 與 Service Worker 版本，降低 iPhone 使用舊快取的機率。
6. 保留原 localStorage 設定鍵，原本已儲存的 Apps Script 網址可繼續使用。

注意：
- 此版本修正的是 GitHub PWA 啟動器。
- Mobile Tenant Manager V6.9.2 Direct Icon 不需要使用，除非改成直接從 Apps Script 加入主畫面。
