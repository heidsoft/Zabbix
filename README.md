# 编译安装
```
yum -y install net-snmp net-snmp-utils net-snmp-devel
yum install libssh2-devel
./configure --enable-server --enable-proxy --enable-agent --enable-java --enable-ipv6 --with-mysql --with-libxml2 -with-net-snmp --with-ssh2 --with-openssl --with-libcurl --with-iconv --prefix=/usr/local/zabbix
```

# 数据库
```
CREATE DATABASE if not exists zabbix  CHARSET utf8 COLLATE utf8_general_ci;

GRANT ALL PRIVILEGES ON zabbix.* TO 'zabbix'@'localhost' IDENTIFIED BY 'zabbix' WITH GRANT OPTION;
```

# 前端web
```
安装后的PHP:/usr/local/php7
安装后php配置文件测试：
[root@zabbix-server bin]# ./php --ini
Configuration File (php.ini) Path: /etc/php7
Loaded Configuration File:         /etc/php7/php.ini
Scan for additional .ini files in: (none)
Additional .ini files parsed:      (none)
安装后默认的php.ini在/etc/php.ini
将其拷贝打破/etc/php7目录中


```

