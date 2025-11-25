# A Shell Script to install amneziawg-go quick and easily.

## Depends on:

> Will be installed if not exists

1. golang
2. g++ gcc make
3. qrencode
4. iptables

## Process
if binaries are not in /usr/bin, it will clone the official repo 
and build it from source.
If VPS does not have resource to build, you can place your binary 
to /usr/bin and run the script, it will not build again.

> Binary name must align amneziawg-go, awg-quick

