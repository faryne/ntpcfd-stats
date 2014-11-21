##新北市消防局報案API ##

### 查詢報案紀錄 ###
- API Endpoint：http://ha2.tw/ntpcfd/api/json
- Request Type：GET
- Response Type：JSON
- 所需參數：
  - service_time：[可選參數]出勤日期，格式為 *YYYY-mm-dd*
  - service_unit[]：[可選參數]出勤分隊，例如 *樹林分隊* 、 *板橋分隊*
  - service_type[]：[可選參數]出勤任務類型，目前只能輸入 *救護*、*火災* 、 *災害* 
- 回傳結果：
  - service_type：出勤任務類型
  - service_unit：出勤分隊
  - service_addr：出勤地址
  - service_time：報案時間
  - lat：出勤地址約略緯度
  - lng：出勤地址約略經度
- 備註：若不帶入任何參數，則取出當天所有報案紀錄。
- 資料來源：http://epaper.tpf.gov.tw/liveview/default.asp
