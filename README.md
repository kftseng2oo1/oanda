# 課堂問答記錄系統（早期版）

記錄每位學生的課堂問答表現：答對、答錯、難度，統計後匯出 Excel 報表。

**線上使用**：https://kftseng2oo1.github.io/oanda/

## 主要功能
- 學生名冊：手動新增，或下載範本後匯入 Excel（姓名、座號、班級），自動略過重複
- 依班級篩選、搜尋學生
- 為學生新增問答紀錄（結果、難度），自動計算得分
- 多選刪除
- 📊 匯出 Excel 報表；💾 下載 JSON 備份、📁 從備份還原
- 自動暫存在 localStorage：`classroomTracker`

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- Excel 讀寫：SheetJS（cdnjs）

## 備註
- 較新的版本在 [tracker](https://github.com/kftseng2oo1/tracker)（多了刪除整個班級、更改題目類別），兩者共用同一個 localStorage key。
