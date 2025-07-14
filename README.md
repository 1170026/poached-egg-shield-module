# Poached Egg Shield Module

ZMK support for the Poached Egg keyboard - a split ortholinear keyboard.

## Features

- 48-key split keyboard layout (6x4 per side)
- Compatible with Seeed XIAO controllers
- ZMK firmware support
- Keymap Editor compatibility

## Keymap Editor Support

This repository now includes full Keymap Editor support. You can use the visual editor to customize your keymap:

1. Open [Keymap Editor](https://keymap-editor.nickcoutsos.com/)
2. Load your keymap from this repository URL:
   `https://github.com/1170026/poached-egg-shield-module`
3. The editor will automatically detect the layout and load your current keymap
4. Make your changes using the visual interface
5. Download the updated keymap file

## Files

- `config/poached_eggs.keymap` - Default keymap configuration
- `config/poached_eggs.json` - Keymap Editor layout definition
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
