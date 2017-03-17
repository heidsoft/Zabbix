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

