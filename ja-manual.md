## 公式サイト

旧サイト : http://bitzeny.org/


新サイト : https://bitzeny.tech/

## BitZenyCore v2.0.1 を インストール

https://github.com/BitzenyCoreDevelopers/bitzeny/releases

(Windows)

bitzeny-2.0.1-win32-setup-unsigned.exe もしくは bitzeny-2.0.1-win64-setup-unsigned.exe

または オンラインウォレット

https://bitzeny.jp/



## CPUMiner-2.6.0

BitZenyをマイニングするためのソフトです

Windows : https://github.com/macchky/cpuminer/releases/tag/v2.6.0

ZNYminer260.zipをインストール

Linux系 : 
```　git clone https://github.com/macchky/cpuminer.git　```



## CPUMiner-2.6.0の設定(Ubuntu)

※Rootではsudoが必要ありません、sudoがうまく動作しない場合はsudoを使わないでください
```
cd cpuminer-master

sudo apt update
 
sudo apt upgrade

sudo apt-get install git

sudo apt-get install libcurl4-openssl-dev gcc-mingw-w64 automake gcc make

./autogen.sh
 
```

### IntelやAMD系のCPU


```
./configure CFLAGS="-O3 -march=native -funroll-loops -fomit-frame-pointer"
 
make
```


### ARM系のCPU

スマートフォンやラズベリーパイなど

```
./configure CFLAGS="-O3 -mfpu=neon"
 
make
```



## Ubuntuでマイニングする
```
./cpuminer-master/minerd -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u 自分のアドレス
```

## Windowsでマイニングする

同じフォルダにstart.batというフォルダを作成、その中に

```
minerd260 -a yescrypt -o stratum+tcp://bitzeny.bluepool.info:3330 -u 自分のアドレス
```

を入力、あとは起動



