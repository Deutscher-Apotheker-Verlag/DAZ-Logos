# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

This repository stores DAZ (Deutsche Apotheker Zeitung) brand logos for use in the DAViD project. It is a static asset repository with no build system, dependencies, or tests.

## Repository Structure

- `eps/` — vector source files (EPS, PSD)
- `svg/` — vector source files for the DAZ+ web badges, taken unmodified from deutsche-apotheker-zeitung.de
- `jpg/` — raster JPEG exports
- `png/` — raster PNG exports

## Using the Logos

Logo files are consumed via raw GitHub URLs:

```
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logo-DAViD/blob/main/jpg/DAZ_Logo1.jpg?raw=true
https://github.com/Deutscher-Apotheker-Verlag/DAZ-Logo-DAViD/blob/main/png/DAZ_Logo1.png?raw=true
```

Replace the filename to reference other variants (`DAZ_Logo2`, `DAZ_Logo3`, `MMP_Logo`).

## Adding New Logo Variants

When adding a new logo, provide the file in all three format directories (eps/, jpg/, png/) and add the corresponding raw GitHub URLs to README.md.

Assets whose source is an SVG (the `DAZ_Plus_Badge_*` files) go into `svg/` instead of `eps/`. Their PNG/JPG exports are rendered at 20× with `sips -s format png -Z <px> file.svg --out file.png` (JPEG: `-s format jpeg -s formatOptions 95`).
