##  今日头条三个参数逆向过程

## [回到总目录](https://github.com/zjw505104341/spider)

### 开始分析

####  直接搜索关键参数
![如图4步走](https://github.com/zjw505104341/spider/blob/master/%E7%BB%83%E6%89%8B%E7%B3%BB%E5%88%97/%E4%BB%8A%E6%97%A5%E5%A4%B4%E6%9D%A1/img/index_1.jpg)

####  打上断点开始调试
![](https://github.com/zjw505104341/spider/blob/master/%E7%BB%83%E6%89%8B%E7%B3%BB%E5%88%97/%E4%BB%8A%E6%97%A5%E5%A4%B4%E6%9D%A1/img/2.jpg)

####   走位进去发现as cp参数加密
![](https://github.com/zjw505104341/spider/blob/master/%E7%BB%83%E6%89%8B%E7%B3%BB%E5%88%97/%E4%BB%8A%E6%97%A5%E5%A4%B4%E6%9D%A1/img/3.jpg)

####   继续走位
![](https://github.com/zjw505104341/spider/blob/master/%E7%BB%83%E6%89%8B%E7%B3%BB%E5%88%97/%E4%BB%8A%E6%97%A5%E5%A4%B4%E6%9D%A1/img/4.jpg)

#### 蒙了  蹦到89了   什么鬼   看不懂 先退为敬

####  退出来直接全局搜索  TAC   嘿嘿    让我发现了  
![](https://github.com/zjw505104341/spider/blob/master/%E7%BB%83%E6%89%8B%E7%B3%BB%E5%88%97/%E4%BB%8A%E6%97%A5%E5%A4%B4%E6%9D%A1/img/5.jpg)


####  直接开撸 js   发现运行js报错，先给下面代码加上
```javascript
navigator = {
    // WT-JS_DEBUG
    appCodeName: "Mozilla",
    appMinorVersion: "0",
    appName: "Netscape",
    appVersion: "5.0 (Windows NT 10.0; WOW64; Trident/7.0; .NET4.0C; .NET4.0E; .NET CLR 2.0.50727; .NET CLR 3.0.30729; .NET CLR 3.5.30729; InfoPath.3; rv:11.0) like Gecko",
    browserLanguage: "zh-CN",
    cookieEnabled: true,
    cpuClass: "x86",
    language: "zh-CN",
    maxTouchPoints: 0,
    msManipulationViewsEnabled: true,
    msMaxTouchPoints: 0,
    msPointerEnabled: true,
    onLine: true,
    platform: "Win32",
    pointerEnabled: true,
    product: "Gecko",
    systemLanguage: "zh-CN",
    userAgent: "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; .NET4.0C; .NET4.0E; .NET CLR 2.0.50727; .NET CLR 3.0.30729; .NET CLR 3.5.30729; InfoPath.3; rv:11.0) like Gecko",
    userLanguage: "zh-CN",
    vendor: "",
    vendorSub: "",
    webdriver: false
}, window = this, window.navigator = navigator;

```

####  逆向结束