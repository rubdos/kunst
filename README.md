<p align="center"><img src="extra/kunst_logo.png"><br><sub>✨ Download and display album art or display embedded album art  ✨</sub></p>

```kunst``` is a deamon that extracts the album art from the songs playing in ```mpd``` and displays them in the a little window. It doesn't loop on a timer, instead it waits for ```mpd``` to send a ```player``` event. When it receives a ```player``` event, it wakes up and extracts the album art of the current playing track. This makes ```kunst```really lightweight and makes it idle at ```~0%``` CPU usage. If there no embbeded album art, it will try to fetch the album art from the internet.


<p align="left">
<img src="https://media.giphy.com/media/5WieRVgCvD4H0V53QY/giphy.gif">
</a>
</p>

## Dependencies
- ```sxiv```
- ```imagemagick```
- ```bash```
- ```ffmpeg```
- ```mpc```

## Installation
**Install using ```make```**
```bash
sudo make install
```
**Install it locally**

Add ```kunst``` to a directory which is in your ```$PATH```

**Install from the AUR**

[AUR](https://aur.archlinux.org/packages/kunst-git/) *(maintained by [networkpanic](https://github.com/networkpanic))*

## Usage

```bash
$ kunst --help
usage: kunst [-h] [--size px] [--music_dir path/to/dir] [--version]
 
┬┌─┬ ┬┌┐┌┌─┐┌┬┐
├┴┐│ ││││└─┐ │
┴ ┴└─┘┘└┘└─┘ ┴
Download and display album art or display embedded album art
 
optional arguments:
   -h, --help            show this help message and exit
   --size                what size to display the album art in
   --music_dir           the music directory which MPD plays from
   --version             show the version of kunst you are using
```

<p align="center">
<a href="https://www.reddit.com/user/SpicyBroseph">
<img src="https://user-images.githubusercontent.com/27065646/53107999-89ec9480-3536-11e9-98a2-9ff416bf4589.png">
</a>
</p>

## License
MIT License

Copyright © 2019 Siddharth Dushantha
