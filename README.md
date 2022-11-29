# 資料庫系統分析
# RDBMS vs NOSQL
### 組成
RDBMS 由資料表組成 需要事先定義好Schema

NOSQL 由collection組成 collection中的document 格式不需要一致
### 什麼時候要用 RDBMS? 什麼時候要用 NOSQL?
當資料需要確保一致性時 較適合使用RDBMS 如銀行的錢轉入轉出 需要同時對兩邊進行操作 或是同時取消 不然會有錢憑空消失

而在整個schema還不確定 或會需要做到頻繁更新時，較適合使用NOSQL
### 選擇
而我最後選擇的是使用RDBMS，由於我們的Schema確定好後就較不會更改，而且資料大多具有一致性，因此最後還是選用RDBMS
## Mysql
![](https://i.imgur.com/i4M7hOC.png)
* 相容於各式各樣的引擎和介面，這也是市場上最成熟的資料庫之一
* 對新手較為友善
* 由於是最流行的資料庫工具之一，很容易在網路上找到支援的資訊
* 但安全機制相較於其他資料庫較為薄弱
* 與PHP配合度最高
* Mysql 商用版會額外提供客戶技術支援服務與許多的工具
* Mysql 免費版並沒有容量限制 而速度則是在有超過128個資料庫連線以上時才會有影響
 ![](https://i.imgur.com/c819D6V.png)


    -- 適合小型專案 如網頁應用程式或是網站
## Oracle
![](https://i.imgur.com/Nkvd9wv.png)
* 效能最高，擁有多項世界紀錄
    *保持windows nt下的tpc-d和tpc-c的世界記錄
* 成本昂貴，免費版功能非常有限
    *(最多支援 2 顆 CPU、2GB 記憶體，只能建立三個資料庫，資料庫大小上限為 12GB)
* 設計目標在於管理大規模的資料表和資料庫

    -- 適合大型專案 個人開發上極少使用Oracle 資料庫

## MSSQL
![](https://i.imgur.com/FOAEa0R.png)
* 價格較MySQL貴，免費版會限制一些功能
    *(數據庫大小限制為 10 GB、CPU 限制為 1 個插槽或 4 個內核)
* 在效能上MSSQL 略勝於 MySQL
* 在介面上與MySQL一樣好上手
* 中小企業常採用

* 與.Net配合度最高
    --與MySQL差不多 適合小型專案
## PostgreSQL
![](https://i.imgur.com/vEn4NvR.png)
* 佔用空間較大
* 效率較低

* 適合高度一致性的資料
* 專為可靠性和資料完整性而設計
* 在windows作業系統下運行沒有MySQL穩定
--較適合如網路銀行等重視資料完整性的專案
---
# **我的選擇**
**MySQL**
對我們的專題來說，使用MySQL 或是 MSSQL 會比使用其他兩個還要再更適合一點
而對我來說，使用MySQL會比使用MSSQL更為熟悉一些，並且其擁有活躍的社群，
在遇到問題時，更容易可以在網路上搜尋到想要的資源。

額外資料:

https://zh.wikipedia.org/zh-tw/ACID

https://shininglionking.blogspot.com/2018/04/rdbms-vs-nosql.html

https://zh.wikipedia.org/zh-tw/CAP%E5%AE%9A%E7%90%86

https://fredwang.blogspot.com/2021/05/mysql-community-mysql.html
