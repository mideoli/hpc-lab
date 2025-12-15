# Node1 Setup (Master)

## Host Configuration
Edit `/etc/hosts`:
```
192.168.46.128 node1
192.168.46.129 node2
```

Set hostname:
```
node1
```

## SSH
```
ssh-keygen -t rsa
ssh-copy-id admin2@node2
```

## Install Packages
```
sudo dnf install -y openmpi openmpi-devel nfs-utils rpcbind autofs indent
```

## Services
```
sudo systemctl start nfs-server
sudo systemctl start rpcbind
sudo systemctl start firewalld
```

> autofs must remain disabled on Node1
