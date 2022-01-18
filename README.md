# edm-project-template 操作手冊

## 介紹

這是一個使用`mjml`框架製作的簡易`edm`模板，之所以使用這個模板是因為要統一並且簡化公司內部`edm`的製作方法。

## 使用方法

由於本模板是使用`mjml`框架製作，所以使用方法就是要透過編寫`mjml`檔案並透過`mjml CLI`來把`mjml`模板轉化為`html`。

請把`edm`的內容以`mjml`語法(詳細語法請至https://mjml.io/)寫在`index.mjml`然後`npm run build`，這樣就可以把`mjml`編譯成`html`。

### edm需要使用背景圖片或image source的場合

多數edm都需要使用圖片，平常專案尚未送至廠商處時，可以先把圖片放在本專案的`img/`資料夾底下，透過相對路徑來讓瀏覽器檢索到圖片。

但是一旦專案要送給廠商時，因為`edm`並<strong>不能</strong>像一般網頁一樣把一整包資料夾傳輸給收信(而是只能收發字串，email伺服器送信的時候等於是把`index.html`的內容以字串送出)，所以`edm`要交稿的時候請<strong>務必</strong>把所有的圖片路徑，包括`Img src`和`Background Url`的圖片全部都上傳到值得信賴的`圖床平台`上(看情況可以選一個公司對外`demo`的資料夾來當作圖床使用)

