(Same Origin Method Execution)SOME ATTACK DEMO 
同源方法执行漏洞

（SOME）是web应用程序攻击方法中的一种，它通过强制受害者在endpoints的域上执行任意页面的脚本方法来滥用回调endpoints(主要是 Flash applets和OAuth 会话的JSONP endpoints—通常重定向到- redirect_uri)。SOME的影响类似于XSS。但是有一些重要且有区别的利用方法。虽然有局限性，但是对特定web功能/网页来说也不限制UI or HTTP 响应头（很重要且有效）。


attacker 构造2个页面 main.html and step1.html

只要发现存在www.leesec.com.callback.php页面类似的漏洞，就是说callback.php页面过滤了xss代码，但是没有过滤opener.test即可利用some











