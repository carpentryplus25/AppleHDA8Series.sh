### NOTE:

* Original ```AppleHDA8Series.sh``` README is [here](https://github.com/Piker-Alpha/AppleHDA8Series.sh)
* Turn ON DEBUG=1 to read more log

### NEW:

- El Capitan support
- Multiple patch pattern support AppleHDA / AppleHDAController each, separate by ```#``` char

```
./AppleHDA8Series.sh -a 892 -l 1
-b AppleHDA:\x8b\x19\xd4\x11,\x92\x08\xec\x10#\x3d\x83\x19\xd4\x11,\x83\xf8\x00\x90\x90
-b AppleHDAController:\x3d\x0c\x0a\x00\x00,\x3d\x0c\x0c\x00\x00#\x3d\x0b\x0c\x00\x00,\x3d\x0c\x0c\x00\x00
-d /Library/Extensions
```

### FIX:

- Default pattern patch
- Patch multiple bytes founded by egrep
- Md5 comparing new & old data

### LIMITATION:

- ~~HDMI with iGPU still doesnt work~~
- ~~Manual repair permissions~~