# WineOS

WineOS is a Debian based distro that just boots into WINE after log-in. Pretty simple, I know. 


```
sudo lb config \
    --mode debian \
    --distribution trixie \
    --architectures amd64 \
    --binary-images iso-hybrid \
    --debian-installer live \
    --debian-installer-gui false \
    --bootloader syslinux \
    --apt-source-archives false \
    --archive-areas "main contrib non-free non-free-firmware" \
    --linux-flavours amd64 \
    --system normal \
    --memtest none
```
then

```
lb build
```