# asus-grouper-config
Create deb package for asus grouper/tilapia on GNU/Linux distros using systemd

Build .deb package:

$ sudo chmod 775 ~/asus-grouper-config/DEBIAN/postinst

$ sudo dpkg-deb --build asus-grouper-config

$ sudo apt install asus-grouper-config.deb
