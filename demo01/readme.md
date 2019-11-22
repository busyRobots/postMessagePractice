## 页面A  通过 iframe 嵌套页面B 的场景；

### 模拟多个域的手段；
* 依赖于npm包 http-server；
* 在不同目录下，启动2个不同端口的静态服务器；

``` shell
# 例如，在demo01的目录下，运行命令 ：
http-serve -p 8080
# 在 demo01/iframe的目录下，运行命令：
http-serve -p 5000
# 即可模拟出一个跨域嵌套的场景
```
或者，可以在项目目录，使用控制台，运行命令打开

```shell
# 安装依赖
yarn; 
# 启动例子
yarn start;
```  

* 在页面上访问：  
```javascript
//因为iframe页面嵌入的地方，是以127.0.0.1 的格式进行书写的

http://127.0.0.1:8080

```