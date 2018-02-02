## About inbestcoin

inbestcoin is a cryptocurrency focused on providing a decentralized mechanism of exchange, and anonymity via untraceable and unlinkable transactions.

You can read more about it at https://coin.inbest.cloud

## Building inbestcoin

### On * nix / OS X

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.59 or later.

You may download them from:

* http://gcc.gnu.org/
* http://www.cmake.org/
* http://www.boost.org/
* Alternatively, it may be possible to install them using a package manager.

To build, change to a directory where this file is located, and run `make`. The resulting executables can be found in `build/release/src`.

**Advanced options:**

* Parallel build: run `make -j<number of threads>` instead of `make`.
* Debug build: run `make build-debug`.
* Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.
* Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`.

### On Windows

Dependencies: MSVC 2015 or later, CMake 2.8.6 or later, and Boost 1.59 or later.

You may download them from:

* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

To build, change to a directory where this file is located, and run these commands:
```
mkdir build
cd build
cmake -G "Visual Studio 14 Win64" ..
```

If you are building on an older processor without AVX support, add the following options to cmake:
```
-DPORTABLE=1 -DWITH_AVX2=0
```

And then build from within MSVC. You may find it helpful to explicitly include Boost paths:
```
cmake.exe -DBOOST_ROOT=C:\boost_1_59_0 -DBOOST_LIBRARYDIR=C:\boost_1_59_0\libs -G "Visual Studio 14 Win64" ..
```
## Community and support

You can find us at:

[Telegram](https://t.me/inbestcoin)

## License

inbestcoin is licensed under the GNU Lesser General Public License v3.0

## Credits

With technology from https://github.com/forknote/cryptonote-generator and https://cryptonote.org/
