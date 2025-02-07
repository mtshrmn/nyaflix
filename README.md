# nyaflix

**nyaflix** is a command-line utility for streaming anime directly from your terminal.
It searches for anime torrents on [nyaa.si](https://nyaa.si) based on your query and provides an interactive selection interface.
Once you select a torrent, *nyaflix* either displays the magnet link or streams the content using **peerflix** with your chosen media player.

## Features

- **Search & Select**: Find anime torrents using your search query.
- **Streaming**: Stream anime via peerflix using your default media player (mpv).
- **Magnet Link Display**: Option to display magnet links without starting the stream.
- **Player Choice**: Use VLC instead of mpv with a simple command-line flag.

## Dependencies

Ensure the following utilities are installed on your system:

- `curl`
- `lynx`
- `fzf`
- `peerflix`
- `parallel`
- `mpv` (default) or `vlc`

## Installation

For arch users, there's a PKGBUILD provided.

For other distributions, just ensure that all the dependencies are installed.
It's a script, you know how to run it.

## Usage

```bash
$ nyaflix --help
nyaflix - stream anime from the terminal
Usage: nyaflix [TITLE] [OPTIONS]

Arguments:
  TITLE

Options:
  -m, --magnet-only                 print magnet of selected file and exit
  --vlc                             use vlc instead of mpv
  --help                            show this message and exit.
```
