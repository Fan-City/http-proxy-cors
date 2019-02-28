# 使用方法

``` bash
# Clone project
git clone http://git.michaelxu.cn/classroom/utils/http-proxy-cors.git

# install dependencies
npm install

# serve with hot reload at localhost:3000
npm start

# 浏览器打开 http://localhost:3000/ ，调用 http://localhost:3000/ 的 BASE_API，都会从 http://10.200.16.225/ 获取数据，然后转发到本地

# 可以修改 /src/utils/http.js 中的 proxy 方法改变转发 URL，或者开启 https 支持

```

# 其他方法
* 使用谷歌的[插件](https://chrome.google.com/webstore/detail/allow-control-allow-origi/nlfbmbojpeacfghkpbjhddihlkkiljbi)解决

* 修改 Chrome（Win7)  
```
# 关闭所有打开的Chrome；  
# 创建Chrome的快捷方式，修改快捷方式的目标为:  
"C:\Program Files\Google\Chrome\Application\chrome.exe"  --disable-web-security  --user-data-dir
# 双击我们创建的Chrome快捷方式，打开Chrome，如图出现“您使用的是不受支持的命令行标记:  
--disable-web-security。稳定性和安全性会有所下降”，表示你取消了跨域限制了，可以随意跨域调用数据了。  
```  

* 修改 Chrome（Mac OS）
```
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --disable-web-security --user-data-dir
or
open -a "Google Chrome"  --disable-web-security
```


