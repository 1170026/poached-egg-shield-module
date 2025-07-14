# Poached Egg Shield Module

ZMK support for the Poached Egg keyboard - a split ortholinear keyboard.

## Keymap Editor Setup

### Option 1: Automatic Layout Parsing (Recommended)
1. Open [Keymap Editor](https://keymap-editor.nickcoutsos.com/)
2. Load your repository: `https://github.com/1170026/poached-egg-shield-module`
3. Go to Settings and enable **"Enable Automatic Layout Parsing"**
4. The editor will automatically detect the layout from the dtsi file

### Option 2: Manual Layout File
If automatic parsing doesn't work well, rename `info.json.backup` to `info.json` to use the manual layout definition.

## Features

- 48-key split keyboard layout (6x4 per side)
- Compatible with Seeed XIAO controllers
- ZMK firmware support
- Keymap Editor compatibility

## Files

- `config/poached_eggs.keymap` - Default keymap configuration
- `config/info.json.backup` - Manual layout definition (backup)
- `config/poached_eggs.zmk.yml` - ZMK metadata for Keymap Editor
- `config/boards/shields/poached_eggs/` - Shield definition files

## Layout

The Poached Egg keyboard features a split ortholinear layout with thumb clusters:

```
┌───┬───┬───┬───┬───┬───┐       ┌───┬───┬───┬───┬───┬───┐
│   │   │   │   │   │   │       │   │   │   │   │   │   │
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│   │   │   │   │   │   │       │   │   │   │   │   │   │
├───┼───┼───┼───┼───┼───┤       ├───┼───┼───┼───┼───┼───┤
│   │   │   │   │   │   │       │   │   │   │   │   │   │
├───┼───┼───┼───┼───┼───┼───┬───┼───┼───┼───┼───┼───┼───┤
│   │   │   │   │   │   │   │   │   │   │   │   │   │   │
└───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┘
```

## Building

To build the firmware:

1. Install ZMK development environment
2. Clone this repository to your ZMK config
3. Build for your target board (typically `seeed_xiao_ble` with `poached_eggs_left` and `poached_eggs_right` shields)

## License

This project follows the original licensing of the upstream repository.

## Contributing

Feel free to submit issues and pull requests to improve the keymap and layout definitions.
