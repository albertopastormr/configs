### [Disable lid close hibernate/suspend](https://askubuntu.com/a/372616)
Open (**sudo**) `/etc/systemd/logind.conf` 

Add a line `HandleLidSwitch=ignore` (make sure it's not commented out!),

Restart the systemd daemon with this command:
`sudo service systemd-logind restart`

### [Bluetooth disabled by default](https://askubuntu.com/a/155886)
Change (**sudo**) `/etc/bluetooth/main.conf`. Change entry `AutoEnable = true` -> `AutoEnable = false`
