# Connecting Wire-guard

To connect to your workloads running in Kloudlite you can use a wireguard device. Here are the steps you need to follow to connect your wireguard.

{% tabs %}
{% tab title="Mac OSX" %}
Step 1: Download wireguard app from Appstore

open : [https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1\&mt=12](https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1\&mt=12)\


Step 2: Get WireGurad config:

1. Go to device section if your profile:  [https://accounts.kloudlite.io/profile/devices](https://accounts.kloudlite.io/profile/devices)
2. You can use existing or create new device in the account
3. Choose the region (region from which you want to connect to server) of the devices
4. Copy generated wireguard config of the region

\
Step 3: Add wireguard interface config to local wireguard

1. Run wireguard application
2. Open Manage Tunnels and add new empty tunnel
3. Paste the wireguard configuration to create tunnel and save\


Step 4: Connect wireguard

Connect to server by choosing the tunnel.
{% endtab %}

{% tab title="Windows" %}
Step 1: Download wireguard MSI Installer from the link below and install the application

open : [https://download.wireguard.com/windows-client/wireguard-installer.exe](https://download.wireguard.com/windows-client/wireguard-installer.exe)\


Step 2: Get WireGurad config:

1. Go to device section if your profile:  [https://accounts.kloudlite.io/profile/devices](https://accounts.kloudlite.io/profile/devices)
2. You can use existing or create new device in the account
3. Choose the region (region from which you want to connect to server) of the devices
4. Copy generated wireguard config of the region

\
Step 3: Add wireguard interface config to local wireguard

1. Run wireguard application
2. Open Manage Tunnels and add new empty tunnel
3. Paste the wireguard configuration to create tunnel and save\


Step 4: Connect wireguard

Connect to server by choosing the tunnel.
{% endtab %}

{% tab title="Linux" %}
Step 1: Install wireguard

```
sudo apt install wireguard wg-quick
```



Step 2: Get WireGurad config:

1. Go to device section if your profile:  [https://accounts.kloudlite.io/profile/devices](https://accounts.kloudlite.io/profile/devices)
2. You can use existing or create new device in the account
3. Choose the region (region from which you want to connect to server) of the devices
4. Copy generated wireguard config of the region



Step 3: Add wireguard interface config to local wireguard

1. Create new config at /etc/kl/interfaces/{tunnel\_name}.config
2. connect:

```
sudo wg-quick up /etc/kl/interfaces/{tunnel_name}.config
```



To disconnect

```
sudo wg-quick down /etc/kl/interfaces/{tunnel_name}.config
```
{% endtab %}
{% endtabs %}

















