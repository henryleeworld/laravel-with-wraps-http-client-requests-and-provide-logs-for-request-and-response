# Laravel 8 包含 HTTP 客戶端請求並提供請求和回應日誌

引入 ahmadwaleed 的 laravel-blanket 套件來擴增包含 HTTP 客戶端請求並提供請求和回應日誌，開發人員需要相關數據和蹤跡，以識別任何來源的使用者影響，並儘速找出受損或所費不貲的程式碼路徑。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產⽣ Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移。
```sh
$ php artisan migrate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/blanket` 來進行日誌監控。

----

## 畫面截圖
![](https://i.imgur.com/LY2OL6x.gif)
> 這是一個高度自以為是的有趣項目，它提供了非常簡單的網路介面和日誌監控
