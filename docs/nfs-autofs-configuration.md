# NFS & autofs

## Node1 (NFS Server)
```
/home/admin1/nfs/cloud *(rw,sync,no_root_squash,no_subtree_check)
```

Apply exports:
```
sudo exportfs -a
```

## Node2 (autofs Client)
`/etc/auto.master`:
```
/home/admin2/nfs /etc/auto.nfs
```

`/etc/auto.nfs`:
```
cloud node1:/home/admin1/nfs/cloud
```
