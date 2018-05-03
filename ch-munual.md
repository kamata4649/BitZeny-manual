※I used Google Translate※

## 官方网站
旧网站：http://bitzeny.org/

新网站：https://bitzeny.tech/


# BitZenyCore v2.0.1 安装

https://github.com/BitzenyCoreDevelopers/bitzeny/releases

(Windows)

bitzeny-2.0.1-win32-setup-unsigned.exe 或 bitzeny-2.0.1-win64-setup-unsigned.exe

或 OnlineWallet↓

https://bitzeny.jp/



## CPUMiner-2.6.0

它是用于挖掘BitZeny的软件。

Windows : https://github.com/macchky/cpuminer/releases/tag/v2.6.0

安装 ZNYminer260.zip

Linux系 : 
```　git clone https://github.com/macchky/cpuminer.git　```



## CPUMiner-2.6.0 设置(Ubuntu)

※Root不需要sudo，如果sudo不能正常工作，请不要使用sudo
```
cd cpuminer-master

sudo apt update
 
sudo apt upgrade

sudo apt-get install git

sudo apt-get install libcurl4-openssl-dev gcc-mingw-w64 automake gcc make

./autogen.sh
 
```

### Intel AMD系 CPU


```
./configure CFLAGS="-O3 -march=native -funroll-loops -fomit-frame-pointer"
 
make
```


### ARM系のCPU

智能手机 Raspberry Pi etc...

```
./configure CFLAGS="-O3 -mfpu=neon"
 
make
```



## Ubuntu Mining
```
./cpuminer/minerd -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u Your address
```

## Windows Mining
在同一个文件夹中创建一个名为start.bat的文件夹.

```
minerd260 -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u Your address
```
