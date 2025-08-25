# STM32G4xx Project Template

### Dependencies

#### STM32CubeMX

https://www.st.com/en/development-tools/stm32cubeide.html

#### RAW

```shell
sudo apt install cmake make git gcc-arm-none-eabi libnewlib-arm-none-eabi libstdc++-arm-none-eabi-newlib binutils-multiarch gdb-multiarch openocd
```

### Clone

```shell
git clone --recurse-submodules https://github.com/pashamray/stm32g4xx_project_template
```

### Build

For debug build:
```shell
cmake -DCMAKE_TOOLCHAIN_FILE=cubeide-gcc.cmake  -S ./ -B build/Debug -GNinja -DCMAKE_BUILD_TYPE=Debug
```

```
cmake --build build/Debug
```

For release build:
```shell
cmake -DCMAKE_TOOLCHAIN_FILE=cubeide-gcc.cmake  -S ./ -B build/Release -GNinja -DCMAKE_BUILD_TYPE=Release
```

```shell
cmake --build build/Release
```
