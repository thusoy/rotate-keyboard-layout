# rotate-keyboard-layout

Simple script to rotate between keyboard layouts in X.


## Usage
    
Pass in the layouts you want to rotate between, then bind that command to a
keyboard shortcut or however you want to rotate between the layouts.

```bash
$ echo Current layout: $(setxkbmap -query | grep layout | cut -d: -f2)
Current layout: en
$ ./rotate_keyboard_layout.py en,no
$ echo Current layout: $(setxkbmap -query | grep layout | cut -d: -f2)
Current layout: no
$ ./rotate_keyboard_layout.py en,no
$ echo Current layout: $(setxkbmap -query | grep layout | cut -d: -f2)
Current layout: en
```
