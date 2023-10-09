You can add VPNs from the network connections manager. Right-click the network icon in your taskbar or hit start ("win" button) and type "connections". You will find some variation of '[network] connections/configuration'.

There, hit the plus symbol to add new connection. Scroll down to find suitable VPN connection type.

You might be missing the proper plugins. Here is how you install them:

```
sudo apt install network-manager-<plugin_name>
```

Where `<plugin_name>` is (obviously) the name of the plugin. Hit tab twice after typing `sudo apt install network-manager-` to see the list of available plugins. Note that the `-gnome` version is the plugin that provides the GUI (if you install that, it will automatically install the base plugin). And, of course, this is Ubuntu distribution dependant. I.e., this asumes the distro is Gnome based.

Anyway, for simplicity, here is a list of commands to install common plugins:

```
sudo apt install network-manager-openconnect
sudo apt install network-manager-vpnc
sudo apt install network-manager-fortisslvpn
```

...or with gnome:

```
sudo apt install network-manager-openconnect-gnome
sudo apt install network-manager-vpnc-gnome
sudo apt install network-manager-fortisslvpn-gnome
```
