# gnome-boxes-share-folder

## Windows

On the host, share the folder you want to share. (Three dots > `Preferences` > `Devices & Shares`)

On the guest, install `spice-webdavd`. ([Spice-space.org Downloads](https://www.spice-space.org/download.html))

## Linux

On the host, share the folder you want to share. (Three dots > `Preferences` > `Devices & Shares`)

On the guest, install `spice-webdavd`.

> For many distros, you can just search for it on the software manager and install it from there.

> On APT based distros (Ubuntu, Linux Mint e.t.c): `apt install spice-webdavd`

If your shares are not automatically added on the file manager, you can manyally add `127.0.0.1` port `9843` as `Webdav`.

> On Linux Mint: Open `Nemo` (file manager) > `File` > `Connect to server` > `Server`: `127.0.0.1`, `Port`: `9843`, `Type`: `WebDAV`, `Folder`: `/`.
