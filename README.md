# marlin-sovol

Configuration files of Marlin 1.1.x bugfix version for sovol sv01 3d printer.

This is not part of an official firmware check the sovol warranty limitation.

# Notes

The filament runout detector is not activated like in the released source code.

The bed is limited to 285mm instead of 290mm to avoid going outside the bed.

The filament unload as to be done manually to limit clogging issues.

# Extra information

I recommand to backup your firmware before uploading a new one. To do so on a Linux:

avrdude -C/AbsolutePathToConfigFiles/avrdude.conf -v -patmega2560 -cwiring -P/dev/ttyUSB0 -b115200 -D -Uflash:r:/AbsolutePathWhereToBackup/dump.hex:i 

You will/may have to change AbsolutePathToConfigFiles, /dev/ttyUSB0 and AbsolutePathWhereToBackup


