# sysbench fork for risc-v

## Step to build
```bash
git clone https://github.com/dictcp/sysbench
cd sysbench/
git submodule update --init
sudo apt install automake libtool pkg-config make
./autogen.sh
./configure --without-mysql
make -j 4
# sysbench binary is ready at ./src/
# 
# you may run benchmark command like
# ./src/sysbench cpu --threads=1 run
```
