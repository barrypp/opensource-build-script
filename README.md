# opensource-build-script

# gdb

export PATH=/opt/gcc-arm-10.2-2020.11-x86_64-arm-none-linux-gnueabihf/bin:$PATH

#

./configure --host=arm-none-linux-gnueabihf --prefix=/mnt/f/Others/gdb/gdb-10.1_ins

make -j 8

make install

#

./configure --host=arm-none-linux-gnueabihf --prefix=/mnt/f/Others/gdb/gdb-10.1_ins_static CXXFLAGS="-static"

make -j 8

make install
