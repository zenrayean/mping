# mping

mping可以从本机对国内服务器发起ping、路由跟踪测试

### 使用方法

```bash
wget https://raw.githubusercontent.com/zenrayean/mping/master/mping.sh && bash mping.sh
wget https://raw.githubusercontent.com/zenrayean/mping/master/mping.sh | bash
```

生成结果如下：


```bash
---------------------------------------------------------------------------
您的本机IP为：[89.208.xxx.xx,俄罗斯 莫斯科]
正在进行Ping测试，请等待...
---------------------------------------------------------------------------
【四川 电信】 - 61.139.2.69

10 packets transmitted, 10 received, 0% packet loss, time 9011ms
rtt min/avg/max/mdev = 175.868/176.184/178.301/0.890 ms
---------------------------------------------------------------------------
【天津 电信】 - 219.150.32.132

10 packets transmitted, 10 received, 0% packet loss, time 9014ms
rtt min/avg/max/mdev = 151.440/151.993/156.191/1.453 ms
---------------------------------------------------------------------------
【江苏 电信】 - 218.2.2.2

10 packets transmitted, 10 received, 0% packet loss, time 9004ms
rtt min/avg/max/mdev = 131.140/131.427/132.370/0.556 ms
---------------------------------------------------------------------------
【四川 联通】 - 119.6.6.6

10 packets transmitted, 10 received, 0% packet loss, time 9020ms
rtt min/avg/max/mdev = 219.419/220.274/223.815/1.494 ms
---------------------------------------------------------------------------
【河北 联通】 - 202.99.160.68

10 packets transmitted, 10 received, 0% packet loss, time 9015ms
rtt min/avg/max/mdev = 160.475/161.261/164.652/1.277 ms
---------------------------------------------------------------------------
【浙江 联通】 - 221.12.1.227

10 packets transmitted, 10 received, 0% packet loss, time 9015ms
rtt min/avg/max/mdev = 137.538/137.633/137.769/0.377 ms
---------------------------------------------------------------------------
【安徽 移动】 - 211.138.180.2

10 packets transmitted, 10 received, 0% packet loss, time 9013ms
rtt min/avg/max/mdev = 142.817/148.090/150.868/2.003 ms
---------------------------------------------------------------------------
【山东 移动】 - 218.201.96.130

10 packets transmitted, 10 received, 0% packet loss, time 9011ms
rtt min/avg/max/mdev = 170.958/180.617/187.635/7.493 ms
---------------------------------------------------------------------------
【四川 移动】 - 223.87.238.22

10 packets transmitted, 10 received, 0% packet loss, time 9019ms
rtt min/avg/max/mdev = 174.732/175.320/177.393/0.958 ms
---------------------------------------------------------------------------
【广东 移动】 - 211.139.129.222

10 packets transmitted, 10 received, 0% packet loss, time 9012ms
rtt min/avg/max/mdev = 161.062/161.325/161.601/0.569 ms
---------------------------------------------------------------------------
【参数说明】
x% packet loss: 丢包率
min: 最低延迟
avg: 平均延迟
max: 最高延迟
mdev: 平均偏差
---------------------------------------------------------------------------

---------------------------------------------------------------------------
正在进行路由跟踪，请稍后...
---------------------------------------------------------------------------
【四川电信】 - 61.139.2.69

traceroute to 61.139.2.69 (61.139.2.69), 30 hops max, 60 byte packets
 1  *
 2  218.30.49.97  4.93 ms  AS4134  美国 ctamericas.com
 3  59.43.182.106  152.42 ms  *  中国 广东 广州 电信
 4  *
 5  59.43.130.157  154.37 ms  *  中国 广东 广州 电信
 6  59.43.146.218  178.42 ms  *  中国 电信
 7  *
 8  61.139.113.54  176.67 ms  AS4134  中国 四川 成都 电信
 9  ns.sc.cninfo.net (61.139.2.69)  175.93 ms  AS4134  中国 四川 成都 电信

---------------------------------------------------------------------------
【河北 联通】- 202.99.160.68

traceroute to 202.99.160.68 (202.99.160.68), 30 hops max, 60 byte packets
 1  *
 2  218.30.48.61  10.11 ms  AS4134  美国 加利福尼亚州 圣何塞 ctamericas.com
 3  59.43.189.33  131.19 ms  *  中国 上海 电信
 4  59.43.187.61  127.61 ms  *  中国 上海 电信
 5  59.43.138.45  127.48 ms  *  中国 上海 电信
 6  59.43.17.117  158.76 ms  *  中国 北京 电信
 7  59.43.17.126  154.31 ms  *  中国 北京 电信
 8  219.158.40.165  158.52 ms  AS4837  中国 北京 联通
 9  219.158.3.65  157.37 ms  AS4837  中国 北京 联通
10  219.158.9.170  155.47 ms  AS4837  中国 北京 联通
11  202.99.160.214  156.95 ms  AS4837  中国 河北 石家庄 联通
12  61.182.146.82  176.78 ms  AS4837  中国 河北 石家庄 联通
13  221.192.35.2  162.34 ms  AS4837  中国 河北 石家庄 联通
14  202.99.160.68  160.62 ms  AS4837  中国 河北 石家庄 联通

---------------------------------------------------------------------------
【安徽 移动】 - 211.138.180.2

traceroute to 211.138.180.2 (211.138.180.2), 30 hops max, 60 byte packets
 1  *
 2  218.30.48.129  0.98 ms  AS4134  美国 ctamericas.com
 3  59.43.186.217  8.40 ms  *  美国 加利福尼亚州 圣何塞 电信
 4  59.43.182.186  128.05 ms  *  中国 上海 电信
 5  *
 6  59.43.130.201  136.00 ms  *  中国 上海 电信
 7  59.43.80.106  140.13 ms  *  中国 上海 电信
 8  202.97.46.14  132.73 ms  AS4134  中国 上海 电信
 9  *
10  221.176.17.33  129.22 ms  AS9808  中国 上海 移动
11  221.176.27.177  151.86 ms  AS9808  中国 安徽 合肥 移动
12  221.183.13.210  148.72 ms  AS9808  中国 安徽 合肥 移动
13  *
14  *
15  ns1.ah.chinamobile.com (211.138.180.2)  143.25 ms  AS9808  中国 安徽 合肥 移动

---------------------------------------------------------------------------

此结果由mping生成:https://github.com/helloxz/mping
```

### 请我喝一杯咖啡
![](https://i.bmp.ovh/imgs/2019/03/cb349aa4a1b95997.png)

### 联系我
* Blog：[https://www.xiaoz.me/](https://www.xiaoz.me/)
* 社区支持：[https://ttt.sh/](https://ttt.sh/)
* QQ:337003006
