sudo add-apt-repository ppa:bitcoin/bitcoin

sudo apt-get update

sudo apt-get install libdb4.8-dev libdb4.8++-dev

git clone https://github.com/allforminers/Berkeley4.8.git

cd Berkeley4.8

unzip db-4.8.30.zip

cd db-4.8.30/dbinc

nano atomic.h


change txt line for this

147 __atomic_compare_exchange_db((p), (o), (n)) 

179 static inline int __atomic_compare_exchange_db(

save

cd build_unix/

../dist/configure --prefix=/usr/local --enable-cxx

make -j8

make install

Also commonly fixes :
libdb_cxx headers missing ubuntu
found berkeley db other than 4.8, required for portable wallets
berkeley db 4.8 ubuntu