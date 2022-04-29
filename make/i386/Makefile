all:
	sudo mkdir -p /home/cogroid/local/libtool/i386
	cd ../../; \
	export CPPFLAGS="-v -m32 -march=i386"; \
	export CXXFLAGS="-v -m32 -march=i386"; \
	export CFLAGS="-v -m32 -march=i386"; \
	./configure --prefix=/home/cogroid/local/libtool/i386; \
	export CPPFLAGS="-v -m32 -march=i386"; \
	export CXXFLAGS="-v -m32 -march=i386"; \
	export CFLAGS="-v -m32 -march=i386"; \
	make

install:
	cd ../../; \
	sudo make install
