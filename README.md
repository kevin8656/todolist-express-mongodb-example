# 20180119-皓神上課

1.建立一個Express專案，並寫好get/post/patch/delete的api router
https://bignerdcoding.gitbooks.io/express/content/gou-jian-api-jie-kou.html

2.安裝mongoDB環境（Mac）

``` 
# brew install mongoDB
# brew service start mongoldb
```

3.下載robomongo
https://robomongo.org/download

4.在Express專案中安裝mongoose套件
```
# yarn add mongoose
```
http://mongoosejs.com/

5.app.js中加入
```
const mongoose = require('mongoose');
mongoose.connect('mongodb://localhost/test');
```

6.專案內加入dotenv套件，並建立.env檔案將環境變數存入，並且在app.js中引入，改寫
```
mongoose.connect('mongodb://localhost/test');
```

7.修改todo.js中的api post，改為存資料入mongodb，並且使用async

> 參考網址：
>
> **Promise:** http://jazzlion.github.io/2016/06/18/Javascript%E7%9A%84%E9%9D%9E%E5%90%8C%E6%AD%A5%E4%B9%8B%E6%97%85-Part-I/
> 
> **async:** https://jigsawye.com/2016/04/18/understanding-javascript-async-await/