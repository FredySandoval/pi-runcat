<img src="runcat.gif" width="150" align="left" />

# pi-runcat

Is a running cat🐱 for your `PI` loading bar

(Yet another useless cat here..)

## pi install 
```bash
wget -P ~/.local/share/fonts "https://github.com/FredySandoval/pi-runcat/releases/download/v1.0.0/runcat.ttf"
pi install npm:pi-runcat
fc-cache -f

# MacOS
curl -L -o ~/Library/Fonts/runcat.ttf "https://github.com/FredySandoval/pi-runcat/releases/download/v1.0.0/runcat.ttf"
# Then restart the app that needs the font. 
# If it still does not appear, you can refresh macOS font caches with:
atsutil databases -removeUser
```

## Manual Installation

Font installation

```bash
cp -r runcat.ttf ~/.local/share/fonts
fc-cache -f
```

##  uninstall 
```bash
pi remove npm:pi-runcat

rm -r ~/.local/share/fonts/runcat.ttf
fc-cache -f
```

## Ghostty
Add this line to your ghostty config to map PUA codepoints to icomoon font
```bash
font-codepoint-map = U+E900-U+E904=icomoon
```

Inspired by [runcat-text](https://github.com/bzglve/runcat-text)

Security:
[security check](https://www.virustotal.com/gui/file/3c5be14dc51cd0d21b34cbd40fe147ff61480ce03655eb43571008975b395d94/community)
