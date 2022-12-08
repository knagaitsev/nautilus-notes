Installation notes:

```
sudo apt install build-essential cmake python3-pip xorriso mtools

pip3 install wllvm
```

Install qemu from source using the method here:

https://www.qemu.org/download/#source

```
git clone https://gitlab.com/qemu-project/qemu.git
cd qemu
git submodule init
git submodule update --recursive
mkdir build
cd build
mkdir output
../configure --prefix=$PWD/output
make -j
make install
```

Add `build/output/bin` to path

Run:
```
cd scripts
./build_deps.sh
```

Add `dep/local/bin` to path

