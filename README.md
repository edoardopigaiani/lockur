# Lockur

Lockur is an i3lock wrapper that takes a screenshot of the desktop, blurs it and sets it as screen locker.

## Dependencies

- i3lock
- maim
- imagemagick

## Installation

Copy the ```lockur``` binary to ```/usr/bin```

The folder ```/usr/share/lockur``` is used as destination folder for the lock icon, if you want to use one

## Usage

```lockur [options]```

Options:

    -h, --help   This help menu.
    -p, --pixelate   Pixelate the background instead of blur, runs faster."

## Systemd .service file

I also provided a .service file needed if you use systemd. You need to place the file in ```/etc/systemd/system/``` and starting/enbaling it. It will invoke lockur each time you resume your machine from suspension or hybernation.