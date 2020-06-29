# Linux ANSI Escape Sequences

Follow the ANSI escape sequences/code to archive colorized and style text in bash termianl.

## Colored Text (ANSI)

Color | Foreground Value | Background Value
--- | --- | ---
Black | 30 | 40
Red | 31 | 41
Green | 32 | 42
Yellow | 33 | 43
Blue | 34 | 44
Magenta | 35 | 45
Cyan | 36 | 46
White | 37 | 47

## Styled Text (ANSI)

Style | Value
--- | ---
No Style | 0
Bold | 1
Low Intensity | 2
Underline | 4
Blinking | 5 (some terminal not supported)
Reverse | 7
Invisible | 8

## Example
```bash
#!/bin/bash
# This is a testing script

flashred="\033[5;31;40m"
red="\033[31;40m"
none="\033[0m"
echo -e $flashred"ERROR: "$none$red"Something is wrong."$none
```

## Reference
Some terminal cannot blink [link](https://unix.stackexchange.com/questions/269809/blink-codeescape-code-has-been-removed)  
More information on ANSI escape code [link](https://en.wikipedia.org/wiki/ANSI_escape_code)  
