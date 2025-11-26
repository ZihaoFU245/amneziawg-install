# A Shell Script to install amneziawg-go quick and easily.

## Overview
This script installs AmneziaWG using the **userspace Go implementation** (`amneziawg-go`).
It does **NOT** install or require any kernel module. This makes it suitable for:
- VPS environments
- LXC containers
- Systems where kernel module installation is not possible

## What gets downloaded from the internet?
If the binaries are not already present, the script will download and build:
1. **amneziawg-go** - Userspace Go implementation from https://github.com/amnezia-vpn/amneziawg-go
2. **amneziawg-tools** - Command line tools (awg, awg-quick) from https://github.com/amnezia-vpn/amneziawg-tools

## Depends on:

> Will be installed if not exists

1. golang
2. g++ gcc make
3. qrencode
4. iptables

## Process
If the binaries are not in /usr/bin, it will clone the official repo 
and build them from source.
If the VPS does not have the resources to build, you can place your binary 
to /usr/bin and run the script, it will not build again.

> Binary name must align amneziawg-go, awg-quick

