# Development

## Embedded
### `arduino-cli`
#### Post Install Settings
Add user to `uucp` and `lock` groups to avoid having to use `sudo` to program:
```
usermod -aG uucp lock USERNAME
chmod 666 /dev/ttyACM? 
```

Use `lsusb` (requires `pciutils` and `usbutils`) to find bus and device for AVR-ISP and then set:
```
chown root:uucp /dev/bus/usb/BUS#/DEV#
```
### `stm32`

## Others
### `python3`
### `python-pip`
### `nodejs`
### `npm`
### `ruby`
### `rust`

## Build Tools

### `ceedling`
### `cmake`

### `make `

### `meson`

### `ninja`
