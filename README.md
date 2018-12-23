# PTT Library

Forked from [Truth0906/PTTLibrary](https://github.com/Truth0906/PTTLibrary)

## 改動：

1. 增強穩定性，主要用於長期爬文。

2. 改善 `login()` `logout()` `getPost()` `getNewestIndex()`

3. 刪除不穩定的多頻道功能。

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

需求
-------------------
###### Python 3.6

相依函式庫
-------------------
###### paramiko
###### uao

API
-------------------
| API  | 說明|
| :---------- | -----------|
| getVersion   | 取得版本資訊   |
| login   | 登入   |
| logout   | 登出   |
| getPost   | 取得文章資訊   |
| getNewestIndex   | 取得該看板最新的文章編號或者信箱最新信件編號   |
| Log   | 顯示訊息   |
| getErrorCode   | 取得錯誤碼   |
| operatePTT   | 向 PTT 送出操作指令   |

贊助 
-------------------
###### 如果你喜歡，你可以贊助這個專案
###### XMR 贊助位址
###### 448CUe2q4Ecf9tx6rwanrqM9kfCwqpNbhJ5jtrTf9FHqHNq7Lvv9uBoQ74SEaAu9FFceNBr6p3W1yhqPcxPPSSTv2ctufnQ
