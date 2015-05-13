# i2pd-ebuild
A Gentoo ebuild script to automate the installation of the i2pd C++ implementation of i2p.

## Installation
- Create a local overlay using this guide: https://wiki.gentoo.org/wiki/Overlay/Local_overlay
- *sudo mkdir -p /usr/local/portage/net-misc*
- *cd /usr/local/portage/net-msic*
- *sudo git clone https://github.com/jebriggsy/i2p-ebuild.git*
- *sudo mv i2p-ebuild i2p*
- *sudo chown -R portage:portage /usr/local/portage* 
- *sudo emerge net-misc/i2pd*

## Usage
- *cd ~*
- *sudo /etc/init.d/i2pd start* (OpenRC)
- *sudo systemctl start i2pd* (Systemd)
- *i2pd [options]* (Direct invocation)

## Start i2pd on boot
- *sudo rc-update add i2pd default* (OpenRC)
- *sudo systemctl enable i2pd.service* (Systemd)

## i2pd config
- Edit */etc/conf.d/i2pd* for command-line options
- Edit */etc/i2pd.conf* for config options

## Advanced usage
- *man i2pd*
