all:
	sudo mkdir -p /home/cogroid/local/libtool/armv7
	cp ./lt__argz.h ../../libltdl/libltdl/
	cd ../../; \
	export LDFLAGS=" -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb"; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	./configure --prefix=/home/cogroid/local/libtool/armv7 --host=arm-linux-androideabi; \

update_makefile:
	cd ../../; \
	export LDFLAGS=" -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb"; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	./make/armv7/chmkfl.sh

build:
	cd ../../; \
	export LDFLAGS=" -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb"; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	make

clean:
	cd ../../; \
	make clean
	rm -f ../../Makefile

install:
	sudo sh -c 'cd ../../; \
	export LDFLAGS=" -v --target=arm-linux-androideabi -march=armv7-a -fPIC -fno-integrated-as --sysroot /home/cogroid/local/android-ndk-r18b/sysroot -isystem /home/cogroid/local/android-ndk-r18b/sysroot/usr/include/arm-linux-androideabi -D__ANDROID_API__=18 -fexceptions -frtti -ffunction-sections -funwind-tables -fstack-protector-strong -Wno-invalid-command-line-argument -Wno-unused-command-line-argument -no-canonical-prefixes -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++/include -I/home/cogroid/local/android-ndk-r18b/sources/cxx-stl/llvm-libc++abi/include -I/home/cogroid/local/android-ndk-r18b/sources/android/support/include -DANDROID -Wa,--noexecstack -Wformat -Werror=format-security -DNDEBUG -O2 -I/usr/include -L/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -B/home/cogroid/local/android-ndk-r18b/platforms/android-18/arch-arm/usr/lib -L/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb -B/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/lib/gcc/arm-linux-androideabi/4.9.x/armv7-a/thumb"; \
	export PATH="/home/cogroid/local/android-ndk-r18b/toolchains/arm-linux-androideabi-4.9/prebuilt/linux-x86_64/bin:${PATH}"; \
	make install; \
	mkdir -p /home/cogroid/local/libtool/armv7/lib; \
	cp -f ./libltdl/.libs/libltdl.so /home/cogroid/local/libtool/armv7/lib/;'
