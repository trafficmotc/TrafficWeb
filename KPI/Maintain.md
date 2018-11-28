# 設備維護率
     
![維護率適用於車輛偵測器(VD)、閉路電視攝影監控(CCTV)、資訊可變標誌(CMS)、自動車輛辨識(AVI)、電子標籤(ETag)](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/KPI計算流程之維護率.png)

## 【總設備即時維護率】

※維護率適用於車輛偵測器(VD)、閉路電視攝影監控(CCTV)、資訊可變標誌(CMS)、自動車輛辨識(AVI)、電子標籤(ETag)

**總設備即時維護率公式：**


$$\mathbf{總設備即時維護率} =\frac{最新XML檔案中維護中的設備數}{建構數} $$


※備註：維護中設備：𝑺𝒕𝒂𝒕𝒖𝒔非0

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/總設備即時維護率.png)  

     
     
## 【單支設備累計維護率】

※維護率適用於車輛偵測器(VD)、閉路電視攝影監控(CCTV)、資訊可變標誌(CMS)、自動車輛辨識(AVI)、電子標籤(ETag)

**單支設備(小時累計/每日累計/當日累計)累計維護率公式：**    

 $$\mathbf{單支設備累計維護率} =\frac{統計期間內設備維護中的總次數}{統計期間內應收總次數} $$

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/單支設備維護率.png)  



## 【總設備平均維護率】

※維護率適用於車輛偵測器(VD)、閉路電視攝影監控(CCTV)、資訊可變標誌(CMS)、自動車輛辨識(AVI)、電子標籤(ETag)

**總設備 (小時累計/每日累計/當日累計)平均維護率公式：**    


 $$\mathbf{總設備 (小時累計/每日累計/當日累計)平均維護率} $$
 $$=統計區間總設備即時維護率之平均$$
 $$=\frac{\sum各檔案維護中的設備數}{建構數 \times 統計區間 應收次數} $$
 $$=\frac{\sum各檔案維護中的設備數}{統計區間應收總次數} $$
 

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/總設備平均維護率.png)  

