# whois查询方法

## whois能查询到什么信息

- 域名所有人
- 域名注册商
- 注册人地址
- 域名注册时间/到期时间
- 域名状态
- 域名DNS服务器
- 域名联系信息
- 等等

## 1、网站查询

第三方：

- *站长工具: `http://whois.chinaz.com/`
- 腾讯WHOIS：`https://whois.cloud.tencent.com/`
- 爱站 `https://whois.aizhan.com/`
- 5118 `https://www.5118.com/`
- 国际域名whois: `https://whois.cnnic.cn/WelcomeServlet`
- *国外多信息查询：`https://www.yougetsignal.com/`
- *国外查询网站：`https://bgp.he.net/dns/`

各大注册商以及第三方站长工具的域名WHOIS信息查询地址：

- 万网WHOIS：`https://whois.aliyun.com/`
- 西部数码WHOIS：`https://whois.west.cn/`
- 新网WHOIS：`http://whois.xinnet.com/domain/whois/index.jsp`
- 纳网WHOIS：`http://whois.nawang.cn/`
- 中资源WHOIS：`https://www.zzy.cn/domain/whois.html`
- 三五互联WHOIS：`https://cp.35.com/chinese/whois.php`
- 新网互联WHOIS：`http://www.dns.com.cn/show/domain/whois/index.do`
- 美橙互联WHOIS：`https://whois.cndns.com/`
- 爱名网WHOIS：`https://www.22.cn/domain/`
- 易名网WHOIS：`https://whois.ename.net/`

## 查询工具

```shell
nmap --script=whois-domain 域名

dmitry -w 域名

whois 域名
```

## whois信息利用

- 在社工库查询邮箱和手机号，获得更多相关联的信息资产，若查到，可尝试登陆服务器商或域名商。
- 利用注册人电话，邮箱等信息通过自由拼接组合成针对网站的社工字典。最后利用字典进行爆破或社工钓鱼，也可用过邮箱和手机号反查找到更多注册域名。
- DNS解析记录可以查ip,查NS、mx邮件交换记录。
- MX记录是邮件服务交换记录，邮件服务经常搭建在目标办公网络，可以让快速我们定位目标核心区域并展开渗透。

查询mx记录,命令：`nslookup -qt=mx baidu.com` (目标地址)
