## 【URI命名原則】


開放資料可透過URL方式取得資料。

###  Web API （application programming interface）表現方式：
   分為網站根目錄（App Root）、資源路徑（Resource Path）和查詢選項（Query Options）![ ](https://ptx.transportdata.tw/PTX/Content/Images/sample_06.jpg)



- 網站根目錄：應用服務的基本網址，主要組成為（Domain）網域名稱和（App）應用程式名稱，並且透過 HTTP 協定連結而形成服務的基本網址。

    Domain: http://traffic.transportdata.tw/MOTC

     App : MOTC或Traffic
     
- 資源路徑：指定資源項目路徑名稱。
 

| 目錄結構 |  意義  |
| :--: | :--------: |
|  Version（版本）|提供服務的版本號。目前提供 v1（第一版），若沒有輸入，則預設最新版本 |
| Service（服務）|依據載具本身提供的服務，例如:鐵道:台鐵（TRA)、高鐵（THSRC)，空運:航空（Aviation），道路:公車（Bus）等等。|
| Application（應用內容）| 根據每個服務而提不同的應用內容，例如:航空:航班資訊（FIDS）和機場資訊（Airport）等。|


###  Traffic API URI設計 

- Traffic Static API URI規則：
   + 取得指定[縣市]發布路段基本資料/Road/Traffic/Section/City/{City}
   + 取得指定[縣市]路況壅塞水準定義資料/Road/Traffic/CongestionLevel/City/{City}
   + 取得指定[縣市]發布路段與基礎路段組合對應資料/Road/Traffic/SectionLink/City/{City}
   + 取得指定[縣市]發布路段線型圖資資料/Road/Traffic/SectionShape/City/{City}
   + 取得[公路總局]發布路段基本資料/Road/Traffic/Section/Highway
   + 取得[公路總局]路況壅塞水準定義資料/Road/Traffic/CongestionLevel/Highway
   + 取得[公路總局]發布路段與基礎路段組合對應資料/Road/Traffic/SectionLink/Highway
   + 取得[公路總局]發布路段線型圖資資料/Road/Traffic/SectionShape/Highway
   + 取得[高速公路局]發布路段基本資料/Road/Traffic/Section/Freeway
   + 取得[高速公路局]路況壅塞水準定義資料/Road/Traffic/CongestionLevel/Freeway
   + 取得[高速公路局]發布路段與基礎路段組合對應資料/Road/Traffic/SectionLink/Freeway
   + 取得[高速公路局]發布路段線型圖資資料/Road/Traffic/SectionShape/Freeway

   + 取得指定[縣市]車輛偵測器基本資料/Road/Traffic/VD/City/{City}
   + 取得指定[縣市]閉路電視攝影監控基本資料/Road/Traffic/CCTV/City/{City}
   + 取得指定[縣市]資訊可變標誌基本資料/Road/Traffic/CMS/City/{City}
   + 取得指定[縣市]自動車輛辨識基本資料/Road/Traffic/AVI/City/{City}
   + 取得指定[縣市]自動車輛辨識配對基本資料/Road/Traffic/AVIPair/City/{City}
   + 取得指定[縣市]電子標籤基本資料/Road/Traffic/ETag/City/{City}
   + 取得指定[縣市]電子標籤配對基本資料/Road/Traffic/ETagPair/City/{City}

   + 取得[公路總局]車輛偵測器基本資料/Road/Traffic/VD/Highway
   + 取得[公路總局]閉路電視攝影監控基本資料/Road/Traffic/CCTV/Highway
   + 取得[公路總局]資訊可變標誌基本資料/Road/Traffic/CMS/Highway
   + 取得[公路總局]自動車輛辨識基本資料/Road/Traffic/AVI/Highway
   + 取得[公路總局]自動車輛辨識配對基本資料/Road/Traffic/AVIPair/Highway
   + 取得[公路總局]電子標籤基本資料/Road/Traffic/ETag/Highway
   + 取得[公路總局]電子標籤配對基本資料/Road/Traffic/ETagPair/Highway

   + 取得[高速公路局]車輛偵測器基本資料/Road/Traffic/VD/Freeway
   + 取得[高速公路局]閉路電視攝影監控基本資料/Road/Traffic/CCTV/Freeway
   + 取得[高速公路局]資訊可變標誌基本資料/Road/Traffic/CMS/Freeway
   + 取得[高速公路局]自動車輛辨識基本資料/Road/Traffic/AVI/Freeway
   + 取得[高速公路局]自動車輛辨識配對基本資料/Road/Traffic/AVIPair/Freeway
   + 取得[高速公路局]電子標籤基本資料/Road/Traffic/ETag/Freeway
   + 取得[高速公路局]電子標籤配對基本資料/Road/Traffic/ETagPair/Freeway



- Traffic Live API URI規則：
   + 取得指定[縣市]路段即時資料/Road/Traffic/Live/City/{City}
   + 取得指定[縣市]車輛偵測器即時資料/Road/Traffic/Live/VD/City/{City}
   + 取得指定[縣市]資訊可變標誌即時資料/Road/Traffic/Live/CMS/City/{City}
   + 取得指定[縣市]自動車輛辨識即時資料/Road/Traffic/Live/AVI/City/{City}
   + 取得指定[縣市]電子標籤即時資料/Road/Traffic/Live/ETag/City/{City}
   + 取得指定[縣市]透過車載GPS探偵產生之路段即時資料/Road/Traffic/Live/GVP/City/{City}
   + 取得指定[縣市]透過手機網路信令探偵產生之路段即時資料/Road/Traffic/Live/CVP/City/{City}
   + 取得[公路總局]路段即時資料/Road/Traffic/Live/Highway
   + 取得[公路總局]車輛偵測器即時資料/Road/Traffic/Live/VD/Highway
   + 取得[公路總局]資訊可變標誌即時資料/Road/Traffic/Live/CMS/Highway
   + 取得[公路總局]自動車輛辨識即時資料/Road/Traffic/Live/AVI/Highway
   + 取得[公路總局]電子標籤即時資料/Road/Traffic/Live/ETag/Highway
   + 取得[公路總局]透過車載GPS探偵產生之路段即時資料/Road/Traffic/Live/GVP/Highway
   + 取得[公路總局]透過手機網路信令探偵產生之路段即時資料/Road/Traffic/Live/CVP/Highway
   + 取得[高速公路局]路段即時資料/Road/Traffic/Live/Freeway
   + 取得[高速公路局]車輛偵測器即時資料/Road/Traffic/Live/VD/Freeway
   + 取得[高速公路局]資訊可變標誌即時資料/Road/Traffic/Live/CMS/Freeway
   + 取得[高速公路局]自動車輛辨識即時資料/Road/Traffic/Live/AVI/Freeway
   + 取得[高速公路局]電子標籤即時資料/Road/Traffic/Live/ETag/Freeway
   + 取得[高速公路局]透過車載GPS探偵產生之路段即時資料/Road/Traffic/Live/GVP/Freeway
   + 取得[高速公路局]透過手機網路信令探偵產生之路段即時資料/Road/Traffic/Live/CVP/Freeway



