Building Zcash for Windows
==========================


This guide has been tested for Debian Stretch, however it should work for Ubuntu and other variants of Debian.

4 GB of RAM is the minimum, and a quad core processor is recommended.

#### Dependencies

    apt-get -y install \
        build-essential pkg-config libc6-dev m4 g++-multilib \
        autoconf libtool ncurses-dev unzip git python python-zmq \
        zlib1g-dev wget bsdmainutils automake mingw-w64 cmake

#### Building

	git clone https://github.com/candunc/zcash.git
	git checkout v1.0.10-1-win-cross
    ./zcutil/build-win.sh

Now, in your ./src/ directory you should have zcashd.exe, zcash-cli.exe, and zcash-tx.exe.
