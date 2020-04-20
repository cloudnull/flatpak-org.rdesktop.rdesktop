# Flatpak for the rdesktop applicaton

This repository contains the flatpak build files for the rdesktop application.

### Build command

``` shell
$ flatpak-builder --repo=org.rdesktop --collection-id=org.rdesktop.Master --force-clean build-dir flatpaks/org.rdesktop/org.rdesktop.json --verbose
```

### Adding the local repository

``` shell
$ flatpak --user remote-add --no-gpg-verify rdesktop org.rdesktop
```

### Installing the rdesktop flatpak

flatpak --user install --assumeyes rdesktop org.rdesktop.rdesktop

## Using the rdesktop flatpak

``` shell
$ flatpak run org.rdesktop.rdesktop --help
```
