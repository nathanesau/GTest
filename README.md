# GTest 

GTest example using CMake.

## Docker

```bash
docker run --rm -it -v "D:/GTest":/app docker.pkg.github.com/nathanesau/docker-qt/qt-static:1.0
apt-get -y install libgtest-dev

# build and run tests
cd /app && mkdir build && cd build && cmake .. && make && test/tests
```

## Ubuntu 20.04

```bash
mkdir build
cd build
cmake ..
make

# run binary
src/stats

# run tests
test/tests
```

## Windows

```bash
mkdir build
cd build
cmake ..
make

# run binary
"src/Debug/stats.exe"

# NOTE: tests aren't compiled on windows
```