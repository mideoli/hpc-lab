# Firewall Configuration

## Node1
```
sudo firewall-cmd --add-rich-rule='rule family="ipv4" source address="192.168.46.129" accept'
sudo firewall-cmd --reload
```

## Node2
```
sudo firewall-cmd --add-rich-rule='rule family="ipv4" source address="192.168.46.128" accept'
sudo firewall-cmd --reload
```
