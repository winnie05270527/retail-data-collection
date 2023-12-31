# 超商資料蒐集

這個專案包括了一系列針對超商（711和全家）的數據進行蒐集的工具和腳本。

從不同來源獲取超商相關的資訊，包括官方網站、Facebook粉專和網路上的門市資訊。

以下是專案中各個腳本的功能和用途：

### 官方網站爬蟲

**腳本名稱：official_seven.py 和 official_family.py**

- 爬取超商官方網站上的最新活動資訊。
- 獲取的資訊包括活動標題、期間、內容和標籤。
- 爬取的資料寫入MySQL資料庫，以供後續分析使用。

### Facebook粉專爬蟲

**腳本名稱：facebook.py**

- 使用第三方套件 `facebook_scraper`爬取超商（711和全家）的Facebook粉專上的發文。
- 獲取的資訊包括發文內容、發文時間、按讚數、留言數、分享數等。
- 爬取的資料寫入MySQL資料庫，以供後續分析使用。

### 門市經緯度

**腳本名稱：location.py**

- 使用 Geocoding API（Google Maps API）將超商門市地址轉換為經緯度坐標。
- 獲取的經緯度資訊寫入MySQL資料庫，以供後續分析使用。

### 月營收

**腳本名稱：revenue.py**

- 將月營收Excel資料寫入MySQL資料庫，以供後續分析使用。
