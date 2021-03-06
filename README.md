## mdmc - Mega Drive Mod Chip (based on MegaDrive++)

mdmc has the following features:

- **USA/JAP/EUR mode switching, including a clock generator**: makes the console region free, and allows it to use all video outputs (RF/Composite/sVideo/RGBs)
- The mod is **switchless** and completely internal, regions can be changed:
    - through the <kbd>Reset</kbd> button: **Keep pushed** to cycle through modes.
    - from the Player 1 controller pad: Press <kbd>Start</kbd> + <kbd>B</kbd> + <kbd>Left</kbd>/<kbd>Up</kbd>/<kbd>Right</kbd> to set your desired mode, NTSC-U / PAL / NTSC-J respectively (geographical position mnemonic).
- The last used mode is saved automatically after 5 seconds and reused at power up.
- Supports a single, dual or RGB LED to indicate the current mode.
- **Reset-From-Pad**: Press <kbd>Start</kbd> + <kbd>A</kbd> + <kbd>B</kbd> + <kbd>C</kbd>.
- Supports consoles with both active-high and active-low reset signals by autosensing (i.e.: **all console revisions**!).

### Installation
Installation instructions for the Arduino are largely the same as MegaDrive++ [head to the wiki](https://github.com/SukkoPera/MegaDrivePlusPlus/wiki). There is an additional piece to install which requires 5 wires, complete installation instructions and pictures will be added soon.

### History
v0.3
* adjustment to PLL config for PAL mode
* checks before region chage: only change if new region is different than current one

v0.2
* slight code cleanup and reorganizing
* removed LCD code to free up SCL/SCA for si5351
* debugging code commented out, otherwise intact

v0.1
* First release, slightly modified MegaDrive++

### License
MegaDrive++ is Copyright &copy; 2015-2019 by SukkoPera.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.
