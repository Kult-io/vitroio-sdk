# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
project adheres to [Semantic Versioning](https://semver.org/).

## [1.5.2]

### Changed

- Node controller initializes timestamp along with communication

## Added

- Timestamp for internal usage in SDK
- Setting of timestamp synchronization interval in node controlller methods

## [1.5.1]

### Changed

- Improved documentation

## Added

- IoTBlock blob size getter

## [1.5.0]

### Changed

- IO expander port used for board revision check
- Attenuation values for ADC count to voltage conversion
- IoT Blocks are now send using provided communication layer

## Added

- Communication abstraction layer for IoT Blocks

## [1.4.0]

### Added

- Predefined sizes of IoTBlock.

### Changed

- IoT Block layout
- ECC object as singletone
- Pins of expander used for board revison check

## [1.3.0]

###  Added
- Support for variable size IoT Block creating and sending.

###  Changed
- IoT block data fields order.
- ECC508.countSHA256 method, to count SHA of more than 64 bytes of data.
- cryptoauthlib ECC init function is now called only once.
- ECC object in IoTBlock source file changed to static.

## [1.2.2]

###  Added
- mbed-cryptoauthlib as submodule
- Patches for mbed-cryptoauthlib
- IoTBlock api
- ECC error handling
- Watchdog class which provides the interface to the Watchdog feature

### Changed
- Memory regions are now defined in SDK,no need to define them in application
   files.
- Node controller doen't need memory regions in constructor.
- Extracted bootloader from vitroio-sdk.
- Extracted ecc508-api from vitroio-sdk.
- Extracted tls_crypto-api from vitroio-sdk.
- Extracted shard-edge-lib from vitroio-sdk

## [1.2.1] - 2020-05-25

###  Added
- Support for closed source static version of Vitro Shard SDK.

## [1.2.0] - 2019-02-10

###  Added
- Support for new protocol communication protocol - firmware ID handling.

## Changed
- Support for new protocol communication protocol - firmware version handling.

## [1.1.0] - 2018-11-26

### Changed

- Change name from `vitroio-embedded-sdk` to `vitro-shard-sdk`

## [1.0.0] - 2018-10-26

### Added

- Firmware developers guide document.
- Features list was added to `README`.

### Changed

- Removed abstraction layer for communication buses - only CAN Bus is supported
for now
- Parameter ID for frame with firmware version changed to `0x30`

### Fixed

- Doxygen documentation was completed, cleanup and unified.

## [0.1.1] - 2018-09-07

### Fixed

- Handling upgrade process after error occurrence

## [0.1.0] - 2018-09-04

### Added

- Initial implementation of debug macros
- Initial implementation of measurement API:
    - abstract classes for drivers and sensors
    - support for registration of sensors
    - support for setting polling time of measurement parameters
- Initial implementation of CAN bus
- Initial implementation of node controller:
    - support for initialization of environment
    - support for initialization of communication with gateway
    - support for firmware upgrade
- Initial implementation of bootloader

[Unreleased]: https://github.com/VitroTech/vitro-shard-sdk/compare/v1.0.0...HEAD
[1.2.0]: https://github.com/VitroTech/vitro-shard-sdk/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/VitroTech/vitro-shard-sdk/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/VitroTech/vitro-shard-sdk/compare/v0.1.1...v1.0.0
[0.1.1]: https://github.com/VitroTech/vitro-shard-sdk/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/VitroTech/vitro-shard-sdk/compare/2878a10257f0f173faee504bc5243e140d36b477...v0.1.0
