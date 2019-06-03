coed
====

## Clone
```
git clone --recursive https://github.com/catchthenewbus/coed.git
```
or
```
git clone https://github.com/catchthenewbus/coed.git
git submodule update --init --recursive
```

## Build on host
```
mkdir build && cd build
cmake ..
make
```

## Build for Raspberry Pi
```
mkdir build && cd build
cmake -DCMAKE_TOOLCHAIN_FILE=../raspberrypi.toolchain ..
make
```

## Run
```
GLOG_logtostderr=1 ./coed # with logging
./coed # without logging
```
