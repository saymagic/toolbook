# Shadowsocks


## 安装

* apt-get install python-pip
* pip install shadowsocks


## 普通启动

* ssserver -p 8836 -k 你设置的密码 -m rc4-md5

* ssserver -p 8836 -k 你设置的密码 -m rc4-md5 -d start
* ssserver -p 8836 -k 你设置的密码 -m rc4-md5 -d stop


## 配置文件

    {
      "server":"你的服务器ip地址",
      "server_port":8388,
      "local_address": "127.0.0.1",
      "local_port":1080,
      "password":"你设置的密码",
      "timeout":300,
      "method":"aes-256-cfb",
      "fast_open": false
    }
### 启动
* ssserver -c /etc/shadowsocks.json
* ssserver -c /etc/shadowsocks.json -d start
* ssserver -c /etc/shadowsocks.json -d stop

## 客户端

[OXS](https://sourceforge.net/projects/shadowsocksgui/files/dist/)
[Windows](https://sourceforge.net/projects/shadowsocksgui/files/dist/)
[Android](https://github.com/shadowsocks/shadowsocks/wiki/Ports-and-Clients#android)
    