# 設備即時率統計說明

![&#x5373;&#x6642;&#x7387;&#x9069;&#x7528;&#x65BC;&#x8ECA;&#x8F1B;&#x5075;&#x6E2C;&#x5668;\(VD\)&#x3001;&#x81EA;&#x52D5;&#x8ECA;&#x8F1B;&#x8FA8;&#x8B58;\(AVI\)&#x3001;&#x96FB;&#x5B50;&#x6A19;&#x7C64;\(ETag\)](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/KPI計算流程之即時率.png)

## 【最新檔案即時率】

※即時率適用於車輛偵測器\(VD\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**最新檔案即時率公式：**

$$\mathbf{最新檔案即時率} =\frac{𝑺𝒚𝒔𝒕𝒆𝒎𝑻𝒊𝒎𝒆−𝑺𝒓𝒄𝑼𝒑𝒅𝒂𝒕𝒆𝑻𝒊𝒎𝒆的時間差低於門檻秒數}{1}$$

※備註：時間差有低於門檻秒數則填1；無則0。

## 【總設備即時率】

※即時率適用於車輛偵測器\(VD\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**總設備即時率公式：**

$$\mathbf{總設備即時率} =\frac{最新XML檔案中符合即時的設備數}{建構數}$$

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/總設備即時率.png)

## 【單支設備即時率】

※即時率適用於車輛偵測器\(VD\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**單支設備\(小時累計/每日累計/當日累計\)即時率公式：**

$$\mathbf{單支設備(小時累計/每日累計/當日累計)即時率} =\frac{統計期間內設備符合即時的總次數}{統計期間內應收總次數}$$

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/單支設備即時率.png)

## 【總設備平均即時率】

※即時率適用於車輛偵測器\(VD\)、自動車輛辨識\(AVI\)、電子標籤\(ETag\)。

**總設備\(小時累計/每日累計/當日累計\)平均即時率公式：**

$$\mathbf{總設備(小時累計/每日累計/當日累計)平均即時率}$$ $$=統計區間總設備符合即時率之平均$$ $$=\frac{\sum各檔案符合即時的設備數}{建構數 \times 統計區間 應收次數}$$ $$=\frac{\sum各檔案符合即時的設備數}{統計區間應收總次數}$$

![ ](https://raw.githubusercontent.com/trafficmotc/UploadInformation/master/KPI/總設備平均即時率.png)
