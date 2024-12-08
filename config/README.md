# DNS config

For when the pi-hole config is not quite done or there are issues with the current setup

## Mac OS
```
sudo nano /etc/hosts
```

## Windows
```
```

# Debug DNS resolution

```
dig http://<service>.pi-cluster.local
dig http://<service>.pi-cluster.local +trace
```

# SSH config

```
nano ~/.ssh/config

# SCP

scp stacks/homer/config.yml pi-cluster-manager:/home/pi/configs/
```
