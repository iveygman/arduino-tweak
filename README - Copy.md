arduino-tweak
======================

Tweaked version of the Arduino codebase (hardware-related code only -- not the IDE)


To use this, check out, clone or otherwise copy the contents of this repository to in place of the contents of /hardware/arduino in your Arduino install folder (will be called something like "arduino-1.5.1r2"). This replaces the default libraries for avr and sam in your Arduino environment.


List of tweaks
--------------

- Added some functions to sam/libraries/Wire: probe() and getInstance()
- Increased buffer size in Wire library for sam to 128 bytes from 32
- Modified Arduino Due valid interrupt lines to attempt to support a few pins that were missed (not fully tested)
