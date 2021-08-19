# xserver-web-vnc

This block uses `x11vnc` and [`novnc`](https://novnc.com/) to setup a web server that gives you VNC control over a running display.

## Usage

Simply visit `http://your-ip-address:9090`. The default password is `poltergeist`. 

## Configuration

| Environment variable | Options | Default | Description |
| --- | --- | --- | --- |
|`DISABLE_PASSWORDS`|`false`, `true`|`false`|Disable all password protection|
|`ACCESS_PASSWORD`|`String`|`poltergeist`|The remote control password for the novnc server. This will allow input (clicking, typing, etc)|
|`VIEW_ONLY`|`false`, `true`|`false`|Enable only view-only mode|
|`VIEW_PASSWORD`|`String`|`bearwitness`|The view-only password for anyone you don't want messing with your cursor|
|`WEB_PORT`|`Number`|`9090`|Default port for novnc|
|`VNC_PORT`|`Number`|`5900`|Default port for x11vnc. You should not need to change this.|
|`DISPLAY`|`String`|`:0`|The local `DISPLAY` variable of your xserver|
