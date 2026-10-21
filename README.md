# DAZ-Logos

This repo provides the DAZ (Deutsche Apotheker Zeitung) logos and badges for [DAViD](https://login.dav-medien.de).

## Structure

| Folder | Content |
|---|---|
| `eps/` | Vector source files of the logos (EPS, PSD) |
| `svg/` | Vector source files of the DAZ+ badges |
| `png/` | PNG exports |
| `jpg/` | JPEG exports |

## How to use the files

The files are referenced via raw GitHub URLs:

```
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/<folder>/<file>?raw=true
```

## Logos

| File | Preview |
|---|---|
| `DAZ_Logo1` | <img src="png/DAZ_Logo1.png" height="40"> |
| `DAZ_Logo2` | <img src="png/DAZ_Logo2.png" height="60"> |
| `DAZ_Logo3` | <img src="png/DAZ_Logo3.png" height="40"> |
| `MMP_Logo` | <img src="png/MMP_Logo.png" height="60"> |

https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Logo1.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Logo2.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Logo3.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/MMP_Logo.jpg?raw=true

https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Logo1.png?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Logo2.png?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Logo3.png?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/MMP_Logo.png?raw=true

## DAZ+ badges

The red and gray DAZ+ badges as used on [deutsche-apotheker-zeitung.de](https://www.deutsche-apotheker-zeitung.de/) to mark DAZ+ articles. The SVGs are the original files from the website; PNG and JPG are rendered from them at 20× (440 × 440 px for the square badges, 1280 × 440 px for the `_Text` variants).

| File | Preview | Colour |
|---|---|---|
| `DAZ_Plus_Badge_Red` | <img src="svg/DAZ_Plus_Badge_Red.svg" height="22"> | `#891E35` |
| `DAZ_Plus_Badge_Gray` | <img src="svg/DAZ_Plus_Badge_Gray.svg" height="22"> | `#686262` |
| `DAZ_Plus_Badge_Red_Text` | <img src="svg/DAZ_Plus_Badge_Red_Text.svg" height="22"> | `#891E35` |
| `DAZ_Plus_Badge_Gray_Text` | <img src="svg/DAZ_Plus_Badge_Gray_Text.svg" height="22"> | `#686262` |

https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/svg/DAZ_Plus_Badge_Red.svg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/svg/DAZ_Plus_Badge_Gray.svg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/svg/DAZ_Plus_Badge_Red_Text.svg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/svg/DAZ_Plus_Badge_Gray_Text.svg?raw=true

https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Plus_Badge_Red.png?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Plus_Badge_Gray.png?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Plus_Badge_Red_Text.png?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/png/DAZ_Plus_Badge_Gray_Text.png?raw=true

https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Plus_Badge_Red.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Plus_Badge_Gray.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Plus_Badge_Red_Text.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logos/blob/main/jpg/DAZ_Plus_Badge_Gray_Text.jpg?raw=true

## Adding new files

Provide each new logo in `eps/` (or `svg/`, if the source is an SVG), `png/` and `jpg/` under the same file name, and add its raw URLs to this README.

PNG and JPG exports from an SVG can be rendered on macOS with `sips`:

```bash
sips -s format png -Z 440 svg/File.svg --out png/File.png
sips -s format jpeg -s formatOptions 95 -Z 440 svg/File.svg --out jpg/File.jpg
```
