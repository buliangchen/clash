## 解决DNS泄露篇

一 、订阅

1.随意转换成clash配置文件（长链接）

2.删除clash订阅链接`false&config=`后面的内容，

3.在config=后加上

```
https://raw.githubusercontent.com/buliangchen/clash/9bae78eaec2d346aa8fe62678d162ba9ac2d6388/nodnsleak
```

拼接成新的地址导入clash即可



#### 电脑端

组策略-管理模板-网络-DNS客户端-禁用只能多宿主名称解析- 双击选择“已启用” 



#### 安卓V2rayNG

1、在设置里

勾选--启用本地DNS 

勾选--启用虚拟DNS 

2、将域名策略改成 Asis

预定义规则改成“绕过局域网及大陆地址而后代理”

重点要 “断开重连” 规则才会生效！

#### clash

1、将设置【覆写】--DNS-策略 改成【强制启用】

​					增强模式改成【Fake-IP 至域名映射】

点击【Name Server】填国内dns：如114.114.114.114(可以添加多个)





#### 小火箭

点击添加配置

https://raw.githubusercontent.com/buliangchen/nodnsleak/main/shadowrocket-rules

下载后使用该配置

将全局路由设置为配置模式即可
