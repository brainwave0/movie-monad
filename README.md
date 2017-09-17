![Movie Monad](https://i.imgur.com/gdsyIMv.png)

# Movie Monad

A desktop video player built with Haskell that uses GStreamer and GTK+.

## Screenshots

![GUI showing Sintel from the Blender Foundation](https://i.imgur.com/SLse3s9.jpg)

## Features

* Local or remote video file playback
    * `file://`
    * `http://`
    * `https://`
* Window size selection
* Fullscreen mode
* Seek
* Play and pause
* Volume
* Keyboard shortcuts
    * Mute toggle
        * `m`
        * `AudioMute`
    * Fullscreen toggle
        * `f`
    * Volume up
        * `Ctrl+ArrowUp` or `Command+ArrowUp` if using a Mac
        * `AudioRaiseVolume`
    * Volume down
        * `Ctrl+ArrowDown` or `Command+ArrowDown` if using a Mac
        * `AudioLowerVolume`
    * Play/pause toggle
        * `Space`
        * `AudioPlay`

## Documentation

[Let's make a GTK Video Player with Haskell](https://lettier.github.io/posts/2017-08-30-haskell-gtk-video-player.html)

## Dependencies

* X11
    * [Windows](https://sourceforge.net/projects/xming/)
    * [Mac](https://www.xquartz.org/)
    * Linux
* [GTK+ >= 3.10](https://www.gtk.org/download/index.php)
* [GStreamer == 1.0](https://gstreamer.freedesktop.org/download/)
* [Haskell](https://www.haskell.org/platform/)

## Install & Run

### Linux

#### AppImage

```bash
# Install GTK+ >= 3.10 (https://www.gtk.org/download/index.php)
# Install GStreamer == 1.0 (https://gstreamer.freedesktop.org/download/)
# Install all of the GStreamer Plugins (https://en.wikipedia.org/wiki/GStreamer#Plug-ins)
# Visit https://github.com/lettier/movie-monad/releases
# * equals the current version
# Download the latest AppImage movie-monad-linux-app-image-*
wget https://github.com/lettier/movie-monad/releases/download/*/movie-monad-linux-app-image-*
chmod a+x movie-monad-linux-app-image-*
./movie-monad-linux-app-image-*
```

### Hackage

```bash
# Install XQuartz (https://www.xquartz.org/) if using Mac OSX or macOS
# Install Xming X Server (https://sourceforge.net/projects/xming/) if using Microsoft Windows
# Install GTK+ >= 3.10 (https://www.gtk.org/download/index.php)
# Install GStreamer == 1.0 (https://gstreamer.freedesktop.org/download/)
# Install all of the GStreamer Plugins (https://en.wikipedia.org/wiki/GStreamer#Plug-ins)
# Install Cabal (https://www.haskell.org/platform/)
# Install Cabal Install (https://www.haskell.org/platform/)
cabal install movie-monad
movie-monad
```

### GitHub

```bash
# Install XQuartz (https://www.xquartz.org/) if using Mac OSX or macOS
# Install Xming X Server (https://sourceforge.net/projects/xming/) if using Microsoft Windows
# Install GTK+ >= 3.10 (https://www.gtk.org/download/index.php)
# Install GStreamer == 1.0 (https://gstreamer.freedesktop.org/download/)
# Install all of the GStreamer Plugins (https://en.wikipedia.org/wiki/GStreamer#Plug-ins)
# Install Git (https://git-scm.com/downloads)
# Install GNU Make (https://www.gnu.org/software/make/)
# Install Haskell (https://www.haskell.org/platform/)
# Install Haksell Stack (https://www.haskell.org/platform/)
git clone https://github.com/lettier/movie-monad.git
cd movie-monad/
make
make install
make run
```

## License

See [LICENSE](LICENSE).

## Copyright

(C) 2017 David Lettier  
[lettier.com](http://www.lettier.com/)
