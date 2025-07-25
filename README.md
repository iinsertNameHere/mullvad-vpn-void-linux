This is a clone of https://gitlab.com/LightSrc/mullvad-vpn-void-linux/

# Mullvad VPN for Void Linux
This repository provides template files, binaries, and installation instructions for setting up [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) on [Void Linux](https://voidlinux.org/).

## Installation Instructions
### Method 1: Adding this Repository to xbps
The easiest way is by adding this repository, which includes pre-built binaries. You can do so by creating a new file and specifying the repository URL.
```bash
echo "repository=https://gitlab.com/LightSrc/mullvad-vpn-void-linux/-/raw/repository-x86_64-glibc" | sudo tee /etc/xbps.d/mullvadvpn-void.conf
```
Once you've created file above, proceed with installing Mullvad VPN using xbps
```bash
sudo xbps-install -S mullvad-vpn
```

### Method 2: Using Void Pilot
If you're interested in setting up multiple applications at once (including Mullvad VPN), consider utilizing the Void Pilot Post Install Utility. You can find more information about it on [GitHub](https://github.com/LightSrc/void-pilot)

### Method 3: Build by using xbps-src
I am not recommending this step, because you will not get updates automatically. Every time when this repository gets updated you need to rebuild from template.
