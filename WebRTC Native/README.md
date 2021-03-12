# Linux-and-Python-Automation-Program

```
$ git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git
```

```
$ export PATH=/path/to/depot_tools:$PATH
```

```
$ echo :$PATH
```

```
$ mkdir -m 711 ~/chromium && cd ~/chromium
```


Linux: ram > 6.4 GB

```
$ fetch --nohooks chromium
```



### 設定 python 指令連結對應的版本解決 bash: python: command not found



首先要先知道 python2.7 在哪裡

```
$ #which python2.7
$ /usr/bin/python2.7
```


去該資料夾，設定連結

```
$ cd /usr/bin
$ ln -s python2.7 python
```


設定完成後看一下目前 python 指令相關的連結

```
$ ls -l python*
```


可以看到目前的設定如:
lrwxrwxrwx 1 root root       9 Mar  2 06:33 python -> python2.7

```
$ ./build/install-build-deps.sh
```
```
$ mkdir webrtc-checkout
```

```
$ cd webrtc-checkout
```

如果不想要完整的回朔歷史記錄，可以通過將加上 --no-history 到來節省大量時間
```
$ fetch --nohooks webrtc
```


```
$ gclient sync
```



## Generating Ninja project files (生成"忍者"項目文件)

[Ninja](https://ninja-build.org/)項目文件使用[GN](https://gn.googlesource.com/gn/+/master/README.md)生成。它放置在您選擇的目錄中，例如out/Debug或out/Release

```
$ gn gen out/Default
```

生成Release版本:





