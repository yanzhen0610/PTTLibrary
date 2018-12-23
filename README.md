![PTTLibrary: A PTT Library in Python](https://i.imgur.com/B1kIMgR.png)
# PTT Library

Forked from [Truth0906/PTTLibrary](https://github.com/Truth0906/PTTLibrary)

## 改動：

1. 增強穩定性，主要用於長期爬文。

2. 改善 `login()` `logout()` `getPost()` `getNewestIndex()`

3. 刪除不穩定的多頻道功能。

#### Do you want PTT in Python? import PTT !

###### PTT Library 是一個由 Python 寫成用來操作 PTT 的函式庫，你可以在任何可以使用 Python 的地方，執行你的 PTT 機器人。
###### 拋棄過往網頁形式的解析，直接登入 PTT 分析最即時的文章與推文，給你最快速的資訊!
###### 支援開放 API，你可以直接使用開放 API 實作你的 PTT 操作指令
###### 測試平台: Windows 10, Ubuntu 18.04
###### 原始碼
###### github: https://github.com/Truth0906/PTTLibrary
###### Pypi: https://pypi.org/project/PTTLibrary/

###### 徵求快樂開發夥伴，歡迎開 issue 討論新想法或者發起 pull request

版本
-------------------
###### 0.7.24

安裝
-------------------
```
pip3 install PTTLibrary
```

基本使用
-------------------
```
from PTTLibrary import PTT

PTTBot = PTT.Library()
ErrCode = PTTBot.login(ID, Password)
if ErrCode != PTT.ErrorCode.Success:
    PTTBot.Log('登入失敗')
    sys.exit()

......

PTTBot.logout()
```

詳細說明
-------------------
###### 請參考 Test.py 有 API 的範例與說明

需求
-------------------
###### Python 3.6

相依函式庫
-------------------
###### progressbar2
###### paramiko
###### uao

未來工作
-------------------
###### 取得我的最愛清單
###### 可蒐集使用者清單
###### 支援 PTT2

API
-------------------
| API  | 說明|
| :---------- | -----------|
| getVersion   | 取得版本資訊   |
| login   | 登入   |
| logout   | 登出   |
| post   | 發佈文章   |
| push   | 推文   |
| mail   | 寄信   |
| getPost   | 取得文章資訊   |
| getNewestIndex   | 取得該看板最新的文章編號或者信箱最新信件編號   |
| giveMoney   | 給予使用者 P 幣   |
| getTime   | 取得 PTT 系統時間   |
| getUser   | 取得使用者資訊   |
| crawlBoard   | 爬蟲 API 可傳入 call back 自訂存檔格式  |
| getMail   | 取得信件資訊   |
| Log   | 顯示訊息   |
| changePassword   | 變更密碼   |
| replyPost   | 回覆文章   |
| throwWaterBall   | 丟水球   |
| delPost   | 刪除文章   |
| operateFriendList   | 操作好友壞人名單   |
| getHistoricalWaterBall   | 查詢歷史水球紀錄   |
| getErrorCode   | 取得錯誤碼   |
| operatePTT   | 向 PTT 送出操作指令   |
| showScreen   | 顯示輸出畫面   |

贊助
-------------------
###### 如果你喜歡，你可以贊助這個專案
###### XMR 贊助位址
###### 448CUe2q4Ecf9tx6rwanrqM9kfCwqpNbhJ5jtrTf9FHqHNq7Lvv9uBoQ74SEaAu9FFceNBr6p3W1yhqPcxPPSSTv2ctufnQ
