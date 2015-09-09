# rpi-config
Raspberry pi config

## Keyboard config
```
$ dpkg-reconfigure keyboard-configuration

select US layout
```

## Network config
```
$ sudo nano /etc/wpa_supplicant/wpa_supplicant.conf

# add at the bottom
network={
    ssid="The_ESSID_from_earlier"
    psk="Your_wifi_password"
}

sudo ifdown wlan0
sudo ifup wlan0
ifconfig wlan0
```
