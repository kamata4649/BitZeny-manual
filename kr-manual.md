# BitZenyCore v2.0.1 설치

https://github.com/BitzenyCoreDevelopers/bitzeny/releases

(Windows)

bitzeny-2.0.1-win32-setup-unsigned.exe 또는 bitzeny-2.0.1-win64-setup-unsigned.exe

또는 Online Wallet

https://bitzeny.jp/



## CPUMiner-2.6.0

BitZeny를 마이닝하기위한 프로그램입니다

Windows : https://github.com/macchky/cpuminer/releases/tag/v2.6.0

ZNYminer260.zip 설치

Linux : 
```　git clone https://github.com/macchky/cpuminer.git　```



## CPUMiner-2.6.0 설정(Ubuntu)

※Root는 sudo가 필요하지 않습니다 sudo가 잘 작동하지 않는 경우 sudo를 사용하지 마십시오※

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

스마트 폰 또는 raspberry pi

```
./configure CFLAGS="-O3 -mfpu=neon"
 
make
```



## Ubuntu Mining
```
./cpuminer-master/minerd -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u 자신의 주소
```

## Windows Mining

같은 폴더에 start.bat라는 폴더를 만들고 그 안에

```
minerd260 -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u 자신의 주소
```


