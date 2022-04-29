[![cogroid.com](https://github.com/cogroid/resources/raw/main/images/banner/cogroid-48.png)](https://cogroid.com)

# GNU libtool

### Packages on Ubuntu 18.04

* [libltdl-dev (2.4.6-2)](https://packages.ubuntu.com/bionic/libltdl-dev)
* [Source Package: libtool (2.4.6-2)](https://packages.ubuntu.com/source/bionic/libtool)

### Prerequisites

###### build-essential

```
sudo apt-get install build-essential
```

###### help2man

```
sudo apt-get install help2man
```

###### GLIBC == 2.27

```
ldd --version
```

* Ubuntu 18.04

###### GCC 32 bit

```
sudo apt install gcc-multilib

sudo apt install g++-multilib
```

###### NDK r18b

* [NDK Downloads](https://developer.android.com/ndk/downloads)
* [NDK r18b for Linux](https://dl.google.com/android/repository/android-ndk-r18b-linux-x86_64.zip)

```
Unzip to folder /home/cogroid/local/android-ndk-r18b
```

###### clang

```
sudo apt install clang
```

### Build for x64 machine

```
cd ${LIBTOOL_DIR}/make/x64
make
```

### Build for i386 machine

```
cd ${LIBTOOL_DIR}/make/i386
make
```

### Build for armv7-a machine

```
cd ${LIBTOOL_DIR}/make/armv7
make
```

---
[Head icons created by Freepik - Flaticon](https://www.flaticon.com/free-icons/head)
