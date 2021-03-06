# Raspberry Pi Pico C++ example project

This is a very basic example for Raspberry Pi Pico.

## Getting Started (Example for Ubuntu 20.04)

Install CMake and cross compiler.

```bash
sudo apt install cmake gcc-arm-none-eabi libnewlib-arm-none-eabi
```

Clone the repository.

```bash
git clone https://github.com/mshr-h/pico-cpp-minimum-example
cd pico-cpp-minimum-example
```

Create build directory.

```bash
mkdir build
cd build
```

Configure and build it.

If`PICO_SDK_PATH` environment variable isn't set, cmake will automatically download [pico-sdk](https://github.com/raspberrypi/pico-sdk) to the `build` directory.

```bash
cmake ..
make -j`nproc`
```

Connect the Pico to the Host PC with pressing the BOOTSEL button.

Copy the binary to Raspberry Pi Pico.

```bash
cp blink.uf2 /path/to/pico_storage
```

The LED on the Pico will start blinking.

## Additional resources

- [raspberrypi/pico-examples](https://github.com/raspberrypi/pico-examples)
- [raspberrypi/pico-sdk](https://github.com/raspberrypi/pico-sdk)
- [Raspberry Pi Pico SDK: Raspberry Pi Pico SDK](https://raspberrypi.github.io/pico-sdk-doxygen/)
- [Raspberry Pi Pico C/C++ SDK](https://datasheets.raspberrypi.org/pico/raspberry-pi-pico-c-sdk.pdf)
