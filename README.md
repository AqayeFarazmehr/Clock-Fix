# Clock-Fix
its just a simple bash code to fix clock in linux

# Why you may ask
because in some old laptops like mine, real time clock isnt working.

# How to
first you need to install "ntp"
```bash

sudo pacman -S ntp
```
then you need to copy clock.sh to /usr/bin/
also copy clock.service to /etc/systemd/system/

its time to give the clock.sh premission
```bash

sudo chmod 755 /usr/bin/clock.sh
```
# Enable and Start the Service
enable it by
```bash

sudo systemctl enable clock.service
```
and start it by
```bash

sudo systemctl start clock.service
```

if you ever feel like to disable it
```bash
sudo systemctl disable clock.service
```
