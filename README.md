# GTest 

<p align="center">
  <a href="https://github.com/nathanesau/GTest" alt="run_tests">
        <img src="https://github.com/nathanesau/GTest/workflows/run_tests/badge.svg" /></a>
  <a href="https://github.com/nathanesau?tab=followers" alt="GitHub followers">
        <img src="https://img.shields.io/github/followers/nathanesau.svg?style=social&label=Follow" /></a>
    <a href="https://GitHub.com/nathanesau/GTest/stargazers/" alt="GitHub stars">
        <img src="https://img.shields.io/github/stars/nathanesau/GTest.svg?style=social&label=Star" /></a>
</p>

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
