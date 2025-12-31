# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a LibreCAD project for designing a man cave layout for 2026. The repository contains CAD drawings in DXF format, which is a CAD data file format developed by Autodesk for enabling data interoperability between AutoCAD and other programs.

## Repository Structure

```
LibreCAD/
  └── man_cave_2026.dxf    # Main CAD drawing file
  └── man_cave_2026.dxf~   # LibreCAD backup file
```

## Working with DXF Files

- **Primary file**: `LibreCAD/man_cave_2026.dxf` is the main CAD drawing
- **Backup files**: Files ending in `~` (e.g., `man_cave_2026.dxf~`) are automatic backups created by LibreCAD
- **File format**: DXF (Drawing Exchange Format) is a text-based CAD format that can be opened with:
  - LibreCAD (open source, cross-platform)
  - AutoCAD
  - Various CAD viewers and editors

## DXF File Structure

DXF files are structured in sections:
- **HEADER**: Drawing metadata and settings (dimensions, units, current layer)
- **TABLES**: Definitions for layers, line types, text styles
- **BLOCKS**: Reusable geometry definitions
- **ENTITIES**: The actual drawing objects (lines, circles, text, etc.)

The current drawing has dimensions of approximately 3115mm x 3665mm with a layer named "STUD_TRACK_LINE".

## Version Control

- Backup files (`*~`) are ignored by Git (see `.gitignore`)
- Only the main `.dxf` file should be committed
- When making changes, LibreCAD will automatically create backup files

## Editing Workflow

1. Open `LibreCAD/man_cave_2026.dxf` in LibreCAD
2. Make your design changes
3. Save the file (LibreCAD will create a backup of the previous version)
4. Commit the updated `.dxf` file to Git
