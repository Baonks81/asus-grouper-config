# asus-grouper-config

This is some service scripts for asus-grouper/tilapia rev.E1565(Nexus 7 2012) which getting from Android LineageOS config:
1. /etc/sysctl.d/10-nexus7.conf - LineageOS
2. /usr/bin/cpufreq.start - ktweak on Android Oneplus6
3. /usr/bin/clear_ram - askubuntu.com or stackoverflow.com
4. /usr/bin/temp_throttle - github.com/sepero/temp-throttle
   
   /usr/bin/cpuinfo_max_freq
   
   /usr/bin/cpuinfo_min_freq
   
   /usr/bin/scaling_available_frequencies

Systemd services:
1. /etc/systemd/system/cpufreq_start.service
2. /etc/systemd/system/temp_throttle.service
3. /etc/systemd/system/clear_ram.service

Create deb package for asus grouper/tilapia on GNU/Linux distros using systemd

Build .deb package:

$ sudo chmod 775 ~/asus-grouper-config/DEBIAN/postinst

$ sudo dpkg-deb --build asus-grouper-config

$ sudo apt install asus-grouper-config.deb
