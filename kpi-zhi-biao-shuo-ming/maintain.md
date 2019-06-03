# 設備維護率統計說明

![&#x7DAD;&#x8B77;&#x7387;&#x9069;&#x7528;&#x65BC;&#x8ECA;&#x8F1B;&#x5075;&#x6E2C;&#x5668;\(VD\)&#x3001;&#x9589;&#x8DEF;&#x96FB;&#x8996;&#x651D;&#x5F71;&#x76E3;&#x63A7;\(CCTV\)&#x3001;&#x8CC7;&#x8A0A;&#x53EF;&#x8B8A;&#x6A19;&#x8A8C;\(CMS\)&#x3001;&#x81EA;&#x52D5;&#x8ECA;&#x8F1B;&#x8FA8;&#x8B58;\(AVI\)&#x3001;&#x96FB;&#x5B50;&#x6A19;&#x7C64;\(ETag\)](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/KPI計算流程之維護率.png)

## 【總設備即時維護率】

※維護率適用於車輛偵測器\(VD\)、閉路電視攝影監控\(CCTV\)、資訊可變標誌\(CMS\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**總設備即時維護率公式：**

$$\mathbf{總設備即時維護率} =\frac{最新XML檔案中維護中的設備數}{建構數}$$

※備註：維護中設備：𝑺𝒕𝒂𝒕𝒖𝒔非0。

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/總設備即時維護率.png)

## 【單支設備累計維護率】

※維護率適用於車輛偵測器\(VD\)、閉路電視攝影監控\(CCTV\)、資訊可變標誌\(CMS\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**單支設備\(小時累計/每日累計/當日累計\)累計維護率公式：**

$$\mathbf{單支設備累計維護率} =\frac{統計期間內設備維護中的總次數}{統計期間內應收總次數}$$

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/單支設備維護率.png)

## 【總設備平均維護率】

※維護率適用於車輛偵測器\(VD\)、閉路電視攝影監控\(CCTV\)、資訊可變標誌\(CMS\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**總設備 \(小時累計/每日累計/當日累計\)平均維護率公式：**

$$\mathbf{總設備 (小時累計/每日累計/當日累計)平均維護率}$$ $$=統計區間總設備即時維護率之平均$$ $$=\frac{\sum各檔案維護中的設備數}{建構數 \times 統計區間 應收次數}$$ $$=\frac{\sum各檔案維護中的設備數}{統計區間應收總次數}$$

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/總設備平均維護率.png)

