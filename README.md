# HPC Lab with Rocky Linux

This project documents a functional High-Performance Computing (HPC) lab built on Rocky Linux using OpenMPI for parallel processing and NFS with autofs for shared storage.

The lab is designed for learning, testing, and small-scale parallel workloads.

# Prerequisites

## Virtualization Platform
- VMWare Workstation 25H2

## Operating System
- I used Rocky Linux 9.6, but it can be replicated using any RHEL-based distro or other Linux Distros

## Required Packages
- openmpi
- openmpi-devel
- nfs-utils
- rpcbind
- autofs
- firewalld

## Network
- Static IP addresses (192.168.46.0/24)
- Hostname resolution via /etc/hosts

# Cluster Topology

| Node  | Hostname | IP Address        | Role |
|------|---------|------------------|------|
| Node1 | node1   | 192.168.46.128   | Master / NFS Server |
| Node2 | node2   | 192.168.46.129   | Compute Node |

## Comunication
- Nodes communicate over a private network with SSH and firewall rules configured.

# Next Steps
- I will be adding to the project Warewulf for workload/containers scheduling; and
- Monitoring with Grafana and Prometheus
