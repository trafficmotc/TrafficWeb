# 支援OData查詢語法

## 【OData語法】

| OData語法 | 說明 | 範例 |
| :--- | :--- | :--- |
| format | 資料格式json、xml、csv | 回傳xml格式 $format=xml |
| select | 回傳資料的某些欄位 | 回傳欄位1 $select= Field1 |
| top | 取最前筆數 | 取前10筆  $top=10 |
| skip | 跳過筆數 | 跳過前100筆  $skip=100 |
| filter | 回傳符合特定表達式的資料 | 車牌號碼等於636-U7的資料 $filter=PlateNumb eq '636-U7' |
| date | 日期 | UpdateTime的日期格式為2015-09-17的資料 $filter=date\(UpdateTime\) eq 2015-09-17 |
| time | 時間 | UpdateTime的時間格式為17:57:00+08:00的資料 $filter=time\(UpdateTime\) eq 11:59:48 |
| contains | 包含 | 車牌號碼包含FA的資料 $filter=contains\(PlateNumb, 'FA'\) |
| all | 所有項目都要符合 | 針對停靠時間資料底下車站代碼，全部的車站代碼為1000的資料就回傳   $filter=StopTimes/all\(d:d/StationID eq '1000'\) |
| any | 其中一項符合 | 針對停靠時間資料底下車站代碼，任一筆的車站代碼為1000的資料就回傳  $filter=StopTimes/any\(d:d/StationID eq '1000'\) |
| orderby {Field asc} | 針對某欄位作升冪 | 針對欄位1作升冪 $orderby= Field1 asc |
| orderby{Field desc} | 針對某欄位作降冪 | 針對欄位1作降冪 $orderby= Field1 desc |

**更多OData服務開發教學**[**請點我**](https://docs.google.com/viewer?url=https://github.com/trafficmotc/Traffic_Web/blob/master/Swagger服務說明上傳參考檔案/資料服務開發實作參考手冊.pdf?raw=true)

