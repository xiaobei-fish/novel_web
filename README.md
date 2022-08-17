# novel_web

使用**Beego框架**进行后端操作编程，并且**爬取**起点小说网的小说数据信息，包括小说名称，简要，封面，作者，类别等信息， 

同时进行后台的操作编程，以及**MVC框架的前后端对接**工作。 

可优化：

通过redis中间件缓存热点key，也可以通过redis中间件维护首页热门博客排行榜避免从数据库中读取。

模糊搜索查询算法优化。



#### conf/app.conf配置

```shell
appname = web
httpport = 8080
runmode = dev

#mysql配置
driverName = mysql
mysqluser = 账号
mysqlpwd = 密码
host = localhost
port = 3306
dbname = 数据库

#session
Sessionon = true
sessionprovider = "file"
sessionname = "web"
sessiongcmaxlifetime = 5400
sessionproviderconfig = "./tmp"
sessioncookielifetime = 5400

#页码展示小说配置
novelListPageNum = 8

#页码展示用户配置
userListPageNum = 8

```

