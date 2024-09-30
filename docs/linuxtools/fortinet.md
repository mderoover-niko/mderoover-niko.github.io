# Fortinet on ubuntu

Step1: Install openfortivpn and its corresponding NetworkManager plugin:

``` sh
sudo apt update
sudo apt install openfortivpn network-manager-fortisslvpn-gnome
sudo systemctl daemon-reload
sudo systemctl restart NetworkManager
```

Step2: Use the gnome-control-center to configure the desired VPN

Step3: profit?
