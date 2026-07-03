# 資料表關聯

[表單總覽](wip.md#表單總覽)

|編號|資料表名稱|編號|工作表名稱|名單來源|其他關連|
|--|--|--|--|--|--|
|F1|[參與意願調查](https://docs.google.com/spreadsheets/d/1dFJ_M3eat-5QGJzTTgddtNwCkPXwnEF2yeBqd5hIU2Q)|F10|表單回覆|-|-|
|F2|[人員資料與團練調查](https://docs.google.com/spreadsheets/d/1Uv-LNNq__V5M1YWl10En8RiOG1vhJyWzkaHw94YCH48)|**F20**|**表單回覆**|-|-|
|F3|[團員半價優惠](https://docs.google.com/spreadsheets/d/1xtQz9T_avZxnjWPBW5okXkPGpNSywtslsCDRWkDCYy4)|F30|表單回覆|-|-|
|F4|[寄票表單](https://docs.google.com/spreadsheets/d/137ed67QpIim21Aj605hPjLrnxJN61gt1qjtLRFWUC0c)|F40|表單回覆|-|-|
|T1|[人事資料總表](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4)|**T11**|**人員總名單**|**💡總源頭**|F20|
|||T12|[校友團費繳交](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4/edit?gid=319775402#gid=319775402)|🔦原生|T11, T18|
|||T13|[團員票領票紀錄](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4/edit?gid=371994255#gid=371994255)|🔦原生|T12|
|||T14|[團員票圖](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4/edit?gid=1696288439#gid=1696288439)|-|-|
|||T15|衛武營後台工作證|T11|F20|
|||T16|衛武營前台工作證|🔦原生|T11, F20|
|||T17|保險同意書|F20|-|
|||T18|入團費繳交紀錄（2025年前）|-|-|
|T2|[出席點名表](https://docs.google.com/spreadsheets/d/1ZqVxk69gxManb5Qf4JO3Z04tJ1CI6iW7U7Wj4kAr6F8)|T21|🌟星團出席表單|T23|F20|
|||T22|🐉龍團出席表單|T23|F20|
|||**T23**|**演出人員名單**|T11|-|
|||T24|出席總計|T23|T21, T22|
|T3|[保險資料](https://docs.google.com/spreadsheets/d/1jks-fXK49GLar90umuvZbhzwTExSF9yfXIaxvXN_hSE)|T31|名單填寫確認|T11|-|
|||T32|保險資訊|F20||

💡 演出或工作人員新增，必須首先將資訊加入於 T11 [人員總名單](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4)。        
🔦 團費與票務紀錄的名單，避免工作表順序調整導致記錄錯誤，因此這兩張的名單直接複製，非用自動關聯。                       
🔦 因此人員新增也需要手動加上於 T12 [校友團費繳交](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4/edit?gid=319775402#gid=319775402)、T13 [團員票領票紀錄](https://docs.google.com/spreadsheets/d/1qtmEVaePaVPPVScvtmeRbesSBFAVDRuCU7Pi3GTUHr4/edit?gid=371994255#gid=371994255)。                
🔦 前台工作證名單 (T16) 亦手動加入。                  

```
                      T18
                       │
                       ▼
F20 ─────► T11 ─────► T12 ──────────► T13   人員總表、團費、團員票
 │          │
 │          │
 │          ├───────► T15、T16              衛武營工作證
 │          │
 │          ▼
 │         T23 ─────► T21、T22 ─────► T24   出席點名統計
 │
 │
 └───────► T17、T32                         保險相關

```