# Spotify

- Spotify launcher not opening on Arch btw (`[2024-03-12T10:47:35Z WARN  spotify_launcher::apt] Download has failed: Broken pipe (os error 32)` if run from the terminal): set `LC_ALL` to an UTF locale before the first run [1](https://bbs.archlinux.org/viewtopic.php?id=290586), [2](https://github.com/kpcyrd/spotify-launcher/issues/24).
