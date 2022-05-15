_APP_PKG_=${APP_PKG}
APP_DIR=/data/data/${_APP_PKG_}

all:
	sudo rm -f /home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a/libc++.so
	sudo ln -s /home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a/libc++_shared.so /home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a/libc++.so
	sudo mkdir -p /home/cogroid/local/libtool/armv7
	cp ./lt__argz.h ../../libltdl/libltdl/
	sudo rm -rf ${APP_DIR}/libtool
	sudo mkdir -p ${APP_DIR}
	sudo ln -s /home/cogroid/local/libtool/armv7 ${APP_DIR}/libtool
	cd ../../; \
	export LDFLAGS=" -stdlib=libc++  -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -L/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a -B/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a  "; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	./configure --prefix=${APP_DIR}/libtool --host=arm-linux-androideabi; \

build:
	cp -f /home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib/crtbegin_so.o ../../
	cp -f /home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib/crtend_so.o ../../
	cp -f /home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib/crtbegin_so.o ../../libltdl/
	cp -f /home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib/crtend_so.o ../../libltdl/
	cd ../../; \
	export LDFLAGS=" -stdlib=libc++  -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -L/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a -B/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a  "; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	make

clean:
	cd ../../; \
	make clean

install:
	sudo sh -c 'cd ../../; \
	export LDFLAGS=" -stdlib=libc++  -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-24/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -L/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a -B/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/libs/armeabi-v7a  "; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	make install;'
