# monero-ebuild
A Gentoo ebuild script to automate the installation of the i2pd C++ implementation of i2p.

## Installation
- Create a local overlay using this guide: https://wiki.gentoo.org/wiki/Overlay/Local_overlay
- *mkdir -p /usr/local/portage/net-misc*
- *cd /usr/local/portage/net-msic*
- *git clone https://github.com/jebriggsy/i2p-ebuild.git*
- *mv i2p-ebuild i2p*
- *chown -R portage:portage /usr/local/portage* 
- *emerge net-p2p/monero*

## Usage
- *cd ~*
- *sudo /etc/init.d/i2pd start*

## Start i2pd on boot
- *sudo rc-update add i2pd default* (OpenRC)
- *sudo systemctl enable i2pd.service* (Systemd)

## i2pd config
- Edit */etc/conf.d/i2pd* for command-line options
- Edit */etc/i2pd.conf* for config options

## Advanced usage
- *man i2pd*
