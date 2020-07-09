# The custom keymap for Mint60

## How to Build
### Docker
- Required:
  - Docker

```
$ docker run -e KEYBOARD=mint60 -e KEYMAP=custom --rm -v $(pwd):/qmk_firmware:rw edasque/qmk_firmware
```

### Makefile
```
$ make mint60:custom
```

## How to Install
```
$ make mint60:custom:avrdude
```
