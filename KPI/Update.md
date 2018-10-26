# 設備即時率




     <img src="https://github.com/trafficmotc/UploadInformation/blob/master/KPI/KPI計算流程之即時率.png" width="200" height="100" />
     
   ![路側設施資料即時率KPI計算流程](https://github.com/trafficmotc/UploadInformation/blob/master/KPI/KPI%E8%A8%88%E7%AE%97%E6%B5%81%E7%A8%8B%E4%B9%8B%E5%8D%B3%E6%99%82%E7%8E%87.png)
     



## 【最新檔案即時率】

      
     

$$\mathbf{最新檔案即時率} =\frac{𝑺𝒚𝒔𝒕𝒆𝒎𝑻𝒊𝒎𝒆−𝑺𝒓𝒄𝑼𝒑𝒅𝒂𝒕𝒆𝑻𝒊𝒎𝒆的時間差低於門檻秒數}{1} $$

備註：時間差有低於門檻秒數則填1；無則0






## 【總設備即時率】

  
   ![總設備即時率](https://github.com/trafficmotc/UploadInformation/blob/master/KPI/%E7%B8%BD%E8%A8%AD%E5%82%99%E5%8D%B3%E6%99%82%E7%8E%87.png)
     
     
     

$$\mathbf{總設備即時率} =\frac{最新XML檔案中符合即時的設備數}{建構數} $$







## 【單支設備(小時累計/每日累計/當日累計)即時率】


  
   ![單支設備(小時累計/每日累計/當日累計)即時率](https://github.com/trafficmotc/UploadInformation/blob/master/KPI/%E5%96%AE%E6%94%AF%E8%A8%AD%E5%82%99%E5%8D%B3%E6%99%82%E7%8E%87.png)




 $$\mathbf{單支設備(小時累計/每日累計/當日累計)即時率} =\frac{統計期間內設備符合即時的總次數}{統計期間內應收總次數} $$






## 【總設備(小時累計/每日累計/當日累計)平均即時率】


  
   ![總設備(小時累計/每日累計/當日累計)平均即時率](https://github.com/trafficmotc/UploadInformation/blob/master/KPI/%E7%B8%BD%E8%A8%AD%E5%82%99%E5%B9%B3%E5%9D%87%E5%8D%B3%E6%99%82%E7%8E%87.png)




 $$\mathbf{總設備(小時累計/每日累計/當日累計)平均即時率} =統計區間總設備符合即時率之平均$$
 $$=\frac{\sum各檔案符合即時的設備數}{建構數 \times 統計區間 應收次數} $$
 $$=\frac{\sum各檔案符合即時的設備數}{統計區間應收總次數} $$
 

