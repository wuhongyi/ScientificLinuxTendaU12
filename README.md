<!-- README.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 三 12月 20 16:19:59 2017 (+0800)
;; Last-Updated: 五 12月 22 21:48:22 2017 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 2
;; URL: http://wuhongyi.cn -->

# README

Scientific Linux 7 下 腾达U12无线网卡驱动安装。

```bash
#root权限下
make
make install
cd wireless_tools
tar -zxcf wireless_tools.30.rtl.tar.gz
cd wireless_tools.30.rtl
make
make install
```


```bash
iwconfig  #查看本机网卡列表，可得到无线网卡名称
iwlist enp0s20u1 scanning  #查看该网卡下可连接的无线网络列表（enp0s20u1为该网卡的名称）
#iwconfig enp0s20u1 essid any  #自动连接可连接的网络，连接其它网络自行百度
iwconfig enp0s20u1 essid "这里填写要连接的无线网络的名称"   #例如 iwconfig enp0s20u1 essid "Wireless PKU"
```



<!-- README.md ends here -->
