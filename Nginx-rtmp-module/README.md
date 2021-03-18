# Linux-and-Python-Automation-Program

https://www.nginx.com/blog/video-streaming-for-remote-learning-with-nginx/

For Debian and Ubuntu
```
sudo apt install libpcre3-dev libssl-dev zlib1g-dev
```
For CentOS, Oracle Linux, and RHEL:

```
sudo yum groupinstall pcre-devel zlib-devel openssl-devel
```

Compiling NGINX with the RTMP Module
https://nginx.org/en/docs/configure.html?_ga=2.186825960.1535535125.1616055787-1969714808.1616055787
```
$ cd /path/to/build/dir*

$ git clone https://github.com/arut/nginx-rtmp-module.git** 

$ git clone https://github.com/nginx/nginx.git** 

$ cd nginx*

$ ./auto/configure --add-module=../nginx-rtmp-module

$ make 

$ sudo make install
```


