# woff2otf folder converter

This is a small utility to convert a folder of WOFF files to the OTF font format. 
It uses Python 3, so you need to have it installed in order to run it.

## Usage

### 1. Prepare Fonts Input Folder
Place all fonts you whant to convert to the `Fonts Input Folder`. See supported folder-structure examples:

```
# Input
~/Downloads/Fonts
├── {fileName}.woff
├── Chrono
│   ├── {fontFileName}.woff
│   ├── ChronoWebBlackItalic.woff
│   └── ChronoWebRegular.woff
├── {fontName}
│   └── {fileName}.woff2
└── ...

# Dist
~/iCloud/Fonts
├── {fileName}.otf
├── Chrono
│   ├── {fontFileName}.otf
│   ├── ChronoWebBlackItalic.otf
│   └── ChronoWebRegular.otf
├── {fontName}
│   └── {fileName}.woff2
└── ...
```

### 2. Run the script

To run the script clone the repo and invoke the `woff2otf.py` from command line. Provide the `input folder path` containing WOFF fonts and `dist folder path folder`

```bash
git clone git@github.com:andriilive/woff2otf-folder.git
cd woff2otf-folder
python3 woff2otf.py ~/Downloads/Fonts ~/iCloud/Fonts
```

## Usefull links 🔗
- [Original Repo](https://github.com/hanikesn/woff2otf)
