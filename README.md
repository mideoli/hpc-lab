# HPC Lab with Rocky Linux

Overview
This project documents a functional High-Performance Computing (HPC) lab built on Rocky Linux using OpenMPI for parallel processing and NFS with autofs for shared storage.

The lab is designed for learning, testing, and small-scale parallel workloads.

# Prerequisites

## Operating System
- Rocky Linux 8 or 9

## Required Packages
- openmpi
- openmpi-devel
- nfs-utils
- rpcbind
- autofs
- firewalld

## Network
- Static IP addresses
- Hostname resolution via /etc/hosts

# Cluster Topology

| Node  | Hostname | IP Address        | Role |
|------|---------|------------------|------|
| Node1 | node1   | 192.168.46.128   | Master / NFS Server |
| Node2 | node2   | 192.168.46.129   | Compute Node |

Nodes communicate over a private network with SSH and firewall rules configured.

# Next Steps
- I will be adding to the project Warewulf for workload scheduling; and
- Monitoring with Grafana and Prometheus
