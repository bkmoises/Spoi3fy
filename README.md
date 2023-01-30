# Spoi3fy

### Table of contents

[**About**](#About)

**Depends**

**How to install**

**Commands**

**License**

## [About][About]
I love the *i3vm* and I love the ease of use it brings using just a keyboard, but it doesn't have many features that interact with the *Spotify* experience, whether it be in terms of notifications or the need to pick up the mouse to change tracks and pause and resume the currently playing tracks.

**Spoi3fy** is a simple collection of my settings that make the experience of using the best music player with the best window manager much better.

### Features

 - Show track title running on *Spotify*  in *i3* status bar.  
 - Pause, resume and change tracks with keyboard with a *VIM* editor lover.

### Example
![enter image description here](https://raw.githubusercontent.com/bkmoises/Spoi3fy/main/example.png)

## Depends
[i3Blocks](https://github.com/vivien/i3blocks) 

    git clone https://github.com/vivien/i3blocks
    cd i3blocks
    ./autogen.sh
    ./configure
    make
    make install

*Access the repository for more details about the project, installation and configuration.*

[Spotify CLI Linux](https://github.com/pwittchen/spotify-cli-linux)

    git clone git@github.com:pwittchen/spotify-cli-linux.git
    cd spotify-cli-linux
    sudo cp spotifycli/spotifycli.py /usr/local/bin/spotifycli

*Access the repository for more details about the project, installation and configuration.*
## How to install
Clone repository to your prefered location.

Move the scripts directory to your *i3* config file (usually placed in `~/.config/i3/`).

Insert the contents of the config file at the end of your config file, path `~/.config/i3/config`.

Still in `~/.config/i3/config` add the following line to the `bar` field.

    bar {
    	status_command i3blocks -c ~/.config/i3/i3blocks.conf 
    }

Insert the contents of the `i3blocks.conf` file in your *i3blocks* configuration file, path `~/.config/i3/i3blocks.conf`.

Restart your *i3vm* environment (usually `Mod + Shift + R`).

## Commands

#### On Normal Mode
| Key | Description |
|--|--|
| `<Mod + s>` | Enter on *Spotify* Mode |

#### On Spotify Mode
| Key | Description |
|--|--|
| `k` | Pause/Resume Track |
| `l` | Next Track |
| `h` | Previous Track |
| `f` | Focus *Spotify* workspace |
| `o` | Open *Spotify* |
| `q` | Close *Spotify* |
| `<C-c>` `<Escape>` `<Return>`| Exit *Spotify* mode |

## License

Copyright (c) 2023 Moisés Andrade

See the file LICENSE for information of licensing and distribution.
