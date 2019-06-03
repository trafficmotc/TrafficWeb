# URI命名原則

交通部即時路況資訊平臺Open API開放資料可透過URL方式取得資料，以下將針對Traffic API URI進行說明。

## 【Web API 表現方式】

Web API （application programming interface）表現方式分為網站根目錄（App Root）、資源路徑（Resource Path）和查詢選項（Query Options）

![ ](https://ptx.transportdata.tw/PTX/Content/Images/sample_06.jpg)

* 網站根目錄：應用服務的基本網址，主要組成為（Domain）網域名稱和（App）應用程式名稱，並且透過 HTTP 協定連結而形成服務的基本網址。

  Domain: [http://traffic.transportdata.tw/MOTC](http://traffic.transportdata.tw/MOTC)

  App : MOTC或Traffic

* 資源路徑：指定資源項目路徑名稱。

| 目錄結構 | 意義 |
| :--- | :--- |
| Version | 提供服務的版本號。目前提供 v2（第二版），若沒有輸入，則預設最新版本 |
| Service | 依據載具本身提供的服務，例如:路況\(Traffic\)。 |
| Application | 根據每個服務而提不同的應用內容，例如:路段（Section）、壅塞水準（CongestionLevel）、基礎路段組合\(SectionLink\)、路段線型圖資\(SectionShape\)、車輛偵測器\(VD\)、閉路電視攝影監控\(CCTV\)、資訊可變標誌\(CMS\)、自動車輛辨識\(AVI\)、自動車輛辨識配對\(AVIPair\)、電子標籤\(ETag\)、電子標籤配對\(ETAGPair\)等。 |

## 【Traffic API URI設計】

* Traffic Static API URI規則：
  * 取得指定\[縣市\]發布路段基本資料/Road/Traffic/Section/City/{City}
  * 取得指定\[縣市\]路況壅塞水準定義資料/Road/Traffic/CongestionLevel/City/{City}
  * 取得指定\[縣市\]發布路段與基礎路段組合對應資料/Road/Traffic/SectionLink/City/{City}
  * 取得指定\[縣市\]發布路段線型圖資資料/Road/Traffic/SectionShape/City/{City}
  * 取得\[公路總局\]發布路段基本資料/Road/Traffic/Section/Highway
  * 取得\[公路總局\]路況壅塞水準定義資料/Road/Traffic/CongestionLevel/Highway
  * 取得\[公路總局\]發布路段與基礎路段組合對應資料/Road/Traffic/SectionLink/Highway
  * 取得\[公路總局\]發布路段線型圖資資料/Road/Traffic/SectionShape/Highway
  * 取得\[高速公路局\]發布路段基本資料/Road/Traffic/Section/Freeway
  * 取得\[高速公路局\]路況壅塞水準定義資料/Road/Traffic/CongestionLevel/Freeway
  * 取得\[高速公路局\]發布路段與基礎路段組合對應資料/Road/Traffic/SectionLink/Freeway
  * 取得\[高速公路局\]發布路段線型圖資資料/Road/Traffic/SectionShape/Freeway
  * 取得指定\[縣市\]車輛偵測器基本資料/Road/Traffic/VD/City/{City}
  * 取得指定\[縣市\]閉路電視攝影監控基本資料/Road/Traffic/CCTV/City/{City}
  * 取得指定\[縣市\]資訊可變標誌基本資料/Road/Traffic/CMS/City/{City}
  * 取得指定\[縣市\]自動車輛辨識基本資料/Road/Traffic/AVI/City/{City}
  * 取得指定\[縣市\]自動車輛辨識配對基本資料/Road/Traffic/AVIPair/City/{City}
  * 取得指定\[縣市\]電子標籤基本資料/Road/Traffic/ETag/City/{City}
  * 取得指定\[縣市\]電子標籤配對基本資料/Road/Traffic/ETagPair/City/{City}
  * 取得\[公路總局\]車輛偵測器基本資料/Road/Traffic/VD/Highway
  * 取得\[公路總局\]閉路電視攝影監控基本資料/Road/Traffic/CCTV/Highway
  * 取得\[公路總局\]資訊可變標誌基本資料/Road/Traffic/CMS/Highway
  * 取得\[公路總局\]自動車輛辨識基本資料/Road/Traffic/AVI/Highway
  * 取得\[公路總局\]自動車輛辨識配對基本資料/Road/Traffic/AVIPair/Highway
  * 取得\[公路總局\]電子標籤基本資料/Road/Traffic/ETag/Highway
  * 取得\[公路總局\]電子標籤配對基本資料/Road/Traffic/ETagPair/Highway
  * 取得\[高速公路局\]車輛偵測器基本資料/Road/Traffic/VD/Freeway
  * 取得\[高速公路局\]閉路電視攝影監控基本資料/Road/Traffic/CCTV/Freeway
  * 取得\[高速公路局\]資訊可變標誌基本資料/Road/Traffic/CMS/Freeway
  * 取得\[高速公路局\]自動車輛辨識基本資料/Road/Traffic/AVI/Freeway
  * 取得\[高速公路局\]自動車輛辨識配對基本資料/Road/Traffic/AVIPair/Freeway
  * 取得\[高速公路局\]電子標籤基本資料/Road/Traffic/ETag/Freeway
  * 取得\[高速公路局\]電子標籤配對基本資料/Road/Traffic/ETagPair/Freeway
* Traffic Live API URI規則：
  * 取得指定\[縣市\]路段即時資料/Road/Traffic/Live/City/{City}
  * 取得指定\[縣市\]車輛偵測器即時資料/Road/Traffic/Live/VD/City/{City}
  * 取得指定\[縣市\]資訊可變標誌即時資料/Road/Traffic/Live/CMS/City/{City}
  * 取得指定\[縣市\]自動車輛辨識即時資料/Road/Traffic/Live/AVI/City/{City}
  * 取得指定\[縣市\]電子標籤即時資料/Road/Traffic/Live/ETag/City/{City}
  * 取得指定\[縣市\]透過車載GPS探偵產生之路段即時資料/Road/Traffic/Live/GVP/City/{City}
  * 取得指定\[縣市\]透過手機網路信令探偵產生之路段即時資料/Road/Traffic/Live/CVP/City/{City}
  * 取得\[公路總局\]路段即時資料/Road/Traffic/Live/Highway
  * 取得\[公路總局\]車輛偵測器即時資料/Road/Traffic/Live/VD/Highway
  * 取得\[公路總局\]資訊可變標誌即時資料/Road/Traffic/Live/CMS/Highway
  * 取得\[公路總局\]自動車輛辨識即時資料/Road/Traffic/Live/AVI/Highway
  * 取得\[公路總局\]電子標籤即時資料/Road/Traffic/Live/ETag/Highway
  * 取得\[公路總局\]透過車載GPS探偵產生之路段即時資料/Road/Traffic/Live/GVP/Highway
  * 取得\[公路總局\]透過手機網路信令探偵產生之路段即時資料/Road/Traffic/Live/CVP/Highway
  * 取得\[高速公路局\]路段即時資料/Road/Traffic/Live/Freeway
  * 取得\[高速公路局\]車輛偵測器即時資料/Road/Traffic/Live/VD/Freeway
  * 取得\[高速公路局\]資訊可變標誌即時資料/Road/Traffic/Live/CMS/Freeway
  * 取得\[高速公路局\]自動車輛辨識即時資料/Road/Traffic/Live/AVI/Freeway
  * 取得\[高速公路局\]電子標籤即時資料/Road/Traffic/Live/ETag/Freeway
  * 取得\[高速公路局\]透過車載GPS探偵產生之路段即時資料/Road/Traffic/Live/GVP/Freeway
  * 取得\[高速公路局\]透過手機網路信令探偵產生之路段即時資料/Road/Traffic/Live/CVP/Freeway

