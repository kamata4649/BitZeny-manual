# BitZenyCore v2.0.1 Install

https://github.com/BitzenyCoreDevelopers/bitzeny/releases

(Windows)

[bitzeny-2.0.1-win32-setup-unsigned.exe]   or   [bitzeny-2.0.1-win64-setup-unsigned.exe]

or OnlineWallet↓

https://bitzeny.jp/



## CPUMiner-2.6.0

It is software for mining BitZeny[※yescrypt-0.5]

Windows : https://github.com/macchky/cpuminer/releases/tag/v2.6.0

ZNYminer260.zip install

Linux : 
```　git clone https://github.com/macchky/cpuminer.git　```



## CPUMiner-2.6.0 setup(Ubuntu)

※Root does not need sudo, please do not use sudo if sudo does not work well.※
```
cd cpuminer-master

sudo apt update
 
sudo apt upgrade

sudo apt-get install git

sudo apt-get install libcurl4-openssl-dev gcc-mingw-w64 automake gcc make

./autogen.sh
 
```

### Intel or AMD CPU


```
./configure CFLAGS="-O3 -march=native -funroll-loops -fomit-frame-pointer"
 
make
```


### ARM CPU

Smart phones and raspberry pi etc...

```
./configure CFLAGS="-O3 -mfpu=neon"
 
make
```



## Ubuntu mining
```
./cpuminer-master/minerd -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u Your address
```

## Windows mining

Create a folder called start.bat in the same folder.

```
minerd260 -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u Your address
```

Start up!!!
