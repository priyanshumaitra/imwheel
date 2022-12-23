# IMWheel

IMWheel is a tool for tweaking mouse wheel behavior, on a per-program basis. It can map mouse wheel input to keyboard input, increase mouse wheel speed, and has support for modifier keys.

- To install ```imwheel``` run the following command.
```
sudo apt-get install imwheel
```
- To read the manual.
```
man imwheel
```
- Run this to start ```imwheel```.
```
imwheel
```
- Run this command to open the ```imwheel``` the config file.
```
gedit ~/.imwheelrc
```
- The configuration below is a config which you can use to fasten your current mouse scroll speed. The mappings are for the entire environment. 
```
".*"
None,      Up,   Button4, 3
None,      Down, Button5, 3
Control_L, Up,   Control_L|Button4
Control_L, Down, Control_L|Button5
Shift_L,   Up,   Shift_L|Button4
Shift_L,   Down, Shift_L|Button5
```
- Or you can setup different configurations for different applications like below.
```
".*-chrome*"
None,       Up,     Up,     3
None,       Down,   Down,   3
```
- Save the file and make sure to run the ```imwheel``` command at the begining of the startup or you can simply setup the command in your startup applications.

**Official site:** https://imwheel.sourceforge.net

**Official README:** https://imwheel.sourceforge.net/README
