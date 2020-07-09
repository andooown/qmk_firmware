# The custom keymap for Ergodox EZ

## How to Build
You can get the pre-built firmwares from [Releases](https://github.com/andooown/qmk_firmware/releases).

### Docker
- Required:
  - Docker

```
$ docker run -e KEYBOARD=ergodox_ez -e KEYMAP=custom --rm -v $(pwd):/qmk_firmware:rw edasque/qmk_firmware
```

### Makefile
```
$ make ergodox:custom
```

## How to Install
- Required:
  - teensy_loader_cli
    - To install, run `brew install teensy_loader_cli`

```
$ teensy_loader_cli --mcu=atmega32u4 -w -v .build/ergodox_ez_custom.hex
```
