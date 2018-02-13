# Introduction
> Socat, as a command line based utility, allows to establish two bidirectional byte streams and transfers data between them.
> Socat will be built for armv7l architecture (Hub-Core). 

# Linux Build Environment Prerequisites
**REQUIREMENT : UBUNTU 16.04 and Python 2.7.12**

### Install The Following pre-requisites - GCC Cross-Compilers and support programs
```sh
$ sudo apt-get install libc6-armel-cross libc6-dev-armel-cross
$ sudo apt-get install binutils-arm-linux-gnueabi
$ sudo apt-get install libncurses5-dev
$ sudo apt-get install gcc-arm-linux-gnueabihf
```

### Socat Build Steps 
```sh
1. Get the tarball and extract it:
	tar xzf socat-1.7.3.2.tar.gz

2. Open terminal and cd "socat-1.7.3.2" directory
	cd socat-1.7.3.2

3. ./configure --build=x86_64-linux-gnu --host=arm-linux-gnueabihf CC=arm-linux-gnueabihf-gcc
   sudo make
   sudo make install

4. Get the executable in /usr/local/bin
	
	
```


