# Node2 Setup (Compute)

## Host Configuration
```
192.168.46.128 node1
192.168.46.129 node2
```

## SSH
```
ssh-keygen -t rsa
ssh-copy-id admin1@node1
```

## Install Packages
```
sudo dnf install -y openmpi openmpi-devel nfs-utils rpcbind autofs indent
```

> NFS server disabled, autofs enabled
