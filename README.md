## Script to handle LEDs in linux
Note: Might have to change it a little if it doesn't work.
### Usage
#### Help
```
$ ./lights -h
usage: lights [-h] command [led] [state]

positional arguments:
  command     on/off/list/set
  led         led_name from list
  state       on or off or brightness

optional arguments:
  -h, --help  show this help message and exit
```
#### List LEDs
```
$ ./lights list
Led_name = Brightness
mute = 0
power = 255
capslock = 0
micmute = 0

```
#### Turn all LEDs off/on:
```
$ ./lights off
- Can't set LED brightness.
- Trying again with root permissions.
[sudo] password for flash: 
Setting brightness of mute LED to 0
Setting brightness of power LED to 0
Setting brightness of capslock LED to 0
Setting brightness of micmute LED to 0
Press Enter to revert.
Setting brightness of mute LED to 0
Setting brightness of power LED to 255
Setting brightness of capslock LED to 0
Setting brightness of micmute LED to 0
```
#### Set brightness of a single LED
```
$ ./lights set power off
- Can't set LED brightness.
- Trying again with root permissions.
Setting brightness of power LED to 0
```
