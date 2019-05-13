# 不可描述的拦截

该教程只能运行在具有内容拦截器的Chromium内核的浏览器内，例如三星浏览器以及Yandex，以及iOS中的Safari浏览器。

## 添加步骤

### 1. 下载内容拦截器

个人推荐AdGuard，界面设计比较新，功能齐全，拦截器多。鉴于在三星浏览器国行系统只能使用Adblock Plus， 虽然不太美观，但也不是不能用。

|   浏览器   |   推荐使用   |
| :--------: | :----------: |
| 三星浏览器 | Adblock Plus |
|   Yandex   |   AdGuard    |
|   Safari   |   AdGuard    |

接下来以Yandex为例

- 首先下载完AdGuard，打开该应用

<img src="https://github.com/Osmole/ContentBlocking/blob/master/Picture/pic1.jpg?raw=true" width="350" alt="pic1" align="center">

- 点击图中的设置，会跳到对应的浏览器进行设置（三星浏览器国内目前只开放了Adblock Plus，其他的无效，可以在浏览器设置里面广告拦截器里面添加）

<img src="https://github.com/Osmole/ContentBlocking/blob/master/Picture/pic2.jpg?raw=true" width="350" alt="pic2" align="center">

- 点击对应的内容拦截器以后，返回AdGuard，在左侧栏内打开用户过滤器

<img src="https://github.com/Osmole/ContentBlocking/blob/master/Picture/pic3.jpg?raw=true" width="350" alt="pic3" align="center">

- 接着进入用户自定义过滤器了

<img src="https://github.com/Osmole/ContentBlocking/blob/master/Picture/pic4.jpg?raw=true" width="350" alt="pic4" align="center">

- 点击导入，输入该仓库的拦截列表地址

https://raw.githubusercontent.com/Osmole/ContentBlocking/master/filterlist.txt

<img src="https://github.com/Osmole/ContentBlocking/blob/master/Picture/pic5.jpg?raw=true" width="350" alt="pic5" align="center">

接着就完成了。

### 规则说明

```
!去除底部安装APP提醒
m.baidu.com##.page-banner
!去除部分广告
baidu.com##div[class^="ec_r"]
!去除百家号
baidu.com##.c-result.result[data-log*="baijiahao"]
!去除短视频推荐
baidu.com##.c-result.result[new_srcid="4660"]
!去除小程序推荐
baidu.com##.c-result.result[new_srcid="38414"]
```



- iOS上需要在`设置`->`Safari浏览器`->`内容拦截器`->`AdGuard`上面打开AdGuard，然后打开AdGuard应用，在自定义规则里面手动添加规则。

- 三星浏览器上具体步骤差不多，Adblock Plus上添加规则步骤为`更多过滤选项`->`添加其他过滤列表` 把拦截列表地址添加进去。添加完成以后得返回到首页点击`更新订阅`，订阅步骤比较慢，得等几分钟。






