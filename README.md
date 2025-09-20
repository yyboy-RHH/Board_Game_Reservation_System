
# 🎮 遊戲預約系統 (Game Reservation System)

這是一個模擬使用者可以透過輸入訊息來 **查詢、預約、取消自己預約的遊戲 **  
實作了兩個版本：  

1. **Dictionary 版本**：使用 Python Dictionary 的方式暫存資料  
2. **SQLite 版本**：使用 SQLite 資料庫,讓遊戲預約狀態永久存在資料庫  

---

## 📌 功能特色
- 查詢尚未被預約的遊戲  
- 預約特定遊戲  
- 取消自己預約的遊戲  
- 模擬多次對話互動  

---

# 🛠 技術細節

## Dictionary 版本
- 使用 Python 的 `dict` 模擬遊戲的預約狀態  
- 適合快速測試與原型設計  

## SQLite 版本
- 使用 Python 進行`sqlite3`資料庫操作  
- 具備永久化特性，程式結束後資料仍會保留在 `game.db`  
- 功能模組化：  
  - `init_games()` 建立資料表並插入資料  
  - `handle_msg()` 處理訊息  

