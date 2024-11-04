
### creates the assets folder on the host

```
ssh pi-cluster-node1
mkdir -p config/homer/assets
mkdir config/homer/assets/images
mkdir config/homer/assets/icons
mkdir config/homer/assets/logo
```

### theme

```
git clone git@github.com:mrpbennett/catppuccin-homer.git
cd catppuccin-homer
scp flavours/catppuccin-frappe.css pi-cluster-node1:/home/pi/config/homer/assets
scp assets/images/backgrounds/romb.png pi-cluster-node1:/home/pi/config/homer/assets/images
scp assets/logos/dark_circle.png pi-cluster-node1:/home/pi/config/homer/assets/logo

# favicons
cd assets/favicons
unzip dark_favicon.zip
rm *.zip
cd -
scp -r assets/favicons pi-cluster-node1:/home/pi/config/homer/assets
```

### refresh config.yml
```

```
