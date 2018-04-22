# BitZenyCore v2.0.1 を インストール

https://github.com/BitzenyCoreDevelopers/bitzeny/releases

(Windows)

bitzeny-2.0.1-win32-setup-unsigned.exe もしくは bitzeny-2.0.1-win64-setup-unsigned.exe

または オンラインウォレット

https://bitzeny.jp/

# CPUMiner-2.6.0

BitZenyをマイニングするためのソフトです

Windows : https://github.com/macchky/cpuminer/releases/tag/v2.6.0

Linux系 : 
	git clone https://github.com/macchky/cpuminer.git


# CPUMiner-2.6.0の設定(Ubuntu)

※Rootではsudoが必要ありません、sudoがうまく動作しない場合はsudoを使わないでください

cd cpuminer-master

sudo apt update
 
sudo apt upgrade

sudo apt-get install git

sudo apt-get install libcurl4-openssl-dev gcc-mingw-w64 automake gcc make

./autogen.sh
 
./configure CFLAGS="-O3 -march=native -funroll-loops -fomit-frame-pointer"
 
make






