# pierced
钉钉内网穿透

TCP 穿透需要在数据库里面执行：
GRANT ALL PRIVILEGES ON *.* TO root@'%' IDENTIFIED BY '123456';
FLUSH PRIVILEGES;
数据库连接命令：
mysql -h vaiwan.com -u root -p -P 1234 //端口号地址



启动工具，执行命令“./ding -config=./ding.cfg -subdomain=域名前缀 端口”，以mac为例：


./ding -config=./ding.cfg -subdomain=qiuwei 8080

2.启动完客户端后，你访问http://abcde.vaiwan.com/xxxxx都会映射到 http://127.0.0.1:8080/xxxxx。
