# FastFetch Config

Fastfetch is a neofetch-like tool for fetching system information and displaying it in a visually appealing way. What it looks like in my Warp terminal.

<img width="850" alt="neural_nebula_dark" src="https://github.com/user-attachments/assets/85c1c1eb-40b1-4e4a-be2d-eac749e30965" />

> [!NOTE]
> You will need to use a Nerd Font from here... https://www.nerdfonts.com/font-downloads

## Installing Fastfetch

```
brew install fastfetch
```

## Theme Config file

```
//{
//  "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/dev/doc/json_schema.json",
//  "modules": [
//   "os",
//    "host",
//    "kernel",
//    "shell",
//    "de",
//    "wm",
//    "terminal",
//    "terminalfont",
//    "terminalsize",
//    "terminaltheme",
//    "break",
//    "colors"
//  ]
//}

{
    "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/dev/doc/json_schema.json",
    "logo": {
        "padding": {
            "top": 2
        }
    },
    "display": {
        "separator": " -> ",
        "constants": [
            "──────────────────────────────"
        ]
    },
    "modules": [
        {
            "type": "custom",
            "format": " {#90}  {#31}  {#32}  {#33}  {#34}  {#35}  {#36}  {#37}  {#38}  {#39}       {#38}  {#37}  {#36}  {#35}  {#34}  {#33}  {#32}  {#31}  {#90}"
        },
        {
            "type": "custom",
            "format": "┌{$1}{$1}┐",
            "outputColor": "90"
        },
        {
            "type": "os",
            "key": "{icon} OS",
            "keyColor": "yellow"
        },
        {
            "type": "kernel",
            "key": "│ ├",
            "keyColor": "yellow"
        },
        {
            "type": "packages",
            "key": "│ ├󰏖",
            "keyColor": "yellow"
        },
        {
            "type": "shell",
            "key": "│ └",
            "keyColor": "yellow"
        },
        {
            "type": "wm",
            "key": " DE/WM",
            "keyColor": "blue"
        },
        {
            "type": "lm",
            "key": "│ ├󰧨",
            "keyColor": "blue"
        },
        {
            "type": "wmtheme",
            "key": "│ ├󰉼",
            "keyColor": "blue"
        },
        {
            "type": "icons",
            "key": "│ ├󰀻",
            "keyColor": "blue"
        },
        {
            "type": "terminal",
            "key": "│ ├",
            "keyColor": "blue"
        },
        {
            "type": "wallpaper",
            "key": "│ └󰸉",
            "keyColor": "blue"
        },
        {
            "type": "host",
            "key": "󰌢 PC",
            "keyColor": "green"
        },
        {
            "type": "cpu",
            "key": "│ ├󰻠",
            "keyColor": "green"
        },
        {
            "type": "gpu",
            "key": "│ ├󰍛",
            "keyColor": "green"
        },
        {
            "type": "disk",
            "key": "│ ├",
            "keyColor": "green"
        },
        {
            "type": "memory",
            "key": "│ ├󰑭",
            "keyColor": "green"
        },
        {
            "type": "swap",
            "key": "│ ├󰓡",
            "keyColor": "green"
        },
        {
            "type": "uptime",
            "key": "│ ├󰅐",
            "keyColor": "green"
        },
        {
            "type": "display",
            "key": "│ └󰍹",
            "keyColor": "green"
        },
        {
            "type": "sound",
            "key": " SND",
            "keyColor": "cyan"
        },
        {
            "type": "player",
            "key": "│ ├󰥠",
            "keyColor": "cyan"
        },
        {
            "type": "media",
            "key": "│ └󰝚",
            "keyColor": "cyan"
        },
        {
            "type": "custom",
            "format": "└{$1}{$1}┘",
            "outputColor": "90"
        },
        "break",
        {
            "type": "custom",
            "format": " {#90}  {#31}  {#32}  {#33}  {#34}  {#35}  {#36}  {#37}  {#38}  {#39}       {#38}  {#37}  {#36}  {#35}  {#34}  {#33}  {#32}  {#31}  {#90}"
        }
    ]
}
```
