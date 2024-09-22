# I2C Scanner

## Description

A utility Arduino script for scanning i2c addresses.

## Requirements

It uses the [platformio](https://platformio.org/) build system to run. 


## How To... 


### Build

`pio run --environment <environment name>`

_Example:_ `pio run --environment esp32doit-devkit-v1`

_NOTE: You can find/add additional environments in the `platformio.ini` file._

### Upload

`pio run --target upload --environment <environment name> --upload-port <port number>`

_Example:_ `pio run -t upload -e esp32doit-devkit-v1 --upload-port COM3`

_NOTE: You can find the available port numbers with `pio device list`._

### Monitor

`pio device monitor --port <port number>`

_Example:_ `pio device monitor --port COM3`

``` PowerShell
pio device monitor --port COM3
--- Terminal on COM3 | 9600 8-N-1
--- Available filters and text transformations: colorize, debug, default, direct, hexlify, log2file, nocontrol, printable, send_on_enter, time
--- More details at https://bit.ly/pio-monitor-filters
--- Quit: Ctrl+C | Menu: Ctrl+T | Help: Ctrl+T followed by Ctrl+H

I2C Scanner
Scanning...
I2C device found at address 0x53  !
I2C device found at address 0x77  !
done

Scanning...
I2C device found at address 0x53  !
I2C device found at address 0x77  !
done
```