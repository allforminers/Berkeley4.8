sudo add-apt-repository ppa:bitcoin/bitcoin

sudo apt-get update

sudo apt-get install libdb4.8-dev libdb4.8++-dev

OR

wget http://download.oracle.com/berkeley-db/db-4.8.30.zip

unzip db-4.8.30.zip

cd db-4.8.30

cd build_unix/

../dist/configure --prefix=/usr/local --enable-cxx

make -j8

make install

Also commonly fixes :
libdb_cxx headers missing ubuntu
found berkeley db other than 4.8, required for portable wallets
berkeley db 4.8 ubuntu