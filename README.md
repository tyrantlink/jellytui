jftui is a simple TUI for Jellyfin for browsing media, and playing it through mpv

Support for Linux and Mac, Windows and other BSD support is untested.

## Requirements
- [mpv](https://mpv.io)

## Installation
### Cargo
```sh
cargo install jftui
```

### From source
```sh
git clone https://github.com/tyrantlink/jftui
cd jftui
cargo build --release
```

## Usage
```sh
jftui
```
On first run, you will be prompted to enter your Jellyfin server URL, username, and password. This information will be stored in `$XDG_CONFIG_HOME/jftui/config.toml` or `$HOME/.config/jftui/config.toml`.

## Keybindings
- `Ctrl + c`: Exit
- `Ctrl + r` | `F5`: Refresh Jellyfin metadata
- `Arrow keys`: Navigate, up and down to scroll, left and right to change pages
- `Page Up` | `Page Down`: Scroll up and down one page
- `Enter`: Play media, or list episodes series
- `Escape`: Exit episode list
- `Ctrl + e`: Toggle episode inclusion in search results
- Any other key: Search, backspace to delete characters, ctrl + backspace to clear search

## Acknowledgements
Name inspired by [jftui](https://github.com/Aanok/jftui) by [Aanok](https://github.com/Aanok)