#### 1.下载

下载好Clash for Linux,
https://github.com/zhaoweih/Clash-Copy

然后解压，点击进去，输入命令./start.sh

再输入 source /etc/profile.d/clash.sh

再输入proxy_on

这样，就开启代理了。

#### 2.开启git代理

使用HTTP代理，输入命令

```C++
git config --global http.proxy http://127.0.1.1:7890
git config --global https.proxy http://127.0.1.1:7890

```

#### 3.开启wget 代理

```C++
sudo gedit ~/.wgetrc

```
在文件中添加以下内容，保存后退出：

```C++

use_proxy = on
http_proxy = http://127.0.0.1:7890
https_proxy = http://127.0.0.1:7890

```
