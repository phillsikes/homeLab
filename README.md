# homeLab
The place for my homeLab overview and documentation as it gets built out.

## The Systems

### clusterPi

Primary Use: 
Setup to run K3s Lightweight Kubernetes to provide local services and stay up to date on current technologies and processes. 1 Master node and 2 Worker nodes set up to run services like WordPress and Pi-Hole, using Persistent Volumes, Horizontal Pod Autoscaling and monitoring.

Hardware
- 3x Raspberry Pi 5 8GB
- 1.5TB SSD Storage

Software
- Ubuntu Server 24.04 LTS
- K3s Lightweight Kubernetes
- Helm package manager
- Prometheus
- Graphana
- Wordpress
- Pi-Hole

### Dell Optiplex 7040 SFF (AKA: the Mule)

Primary Use: 
Currently running as a test mule for trying out new services before implimenting them on the Kubernetets Cluster and preparing for RHCSA certification.

Hardware
- Intel Core i7 6700 Processor
- 32GB RAM
- 1TB SSD

Software
- RHEL 10 Server w/ GUI

## The Network

Hardware
- Unifi Cloud Gateway Ultra
- Unifi Switch 8 60W (8-Port Managed Gigabit Switch with PoE)
- Unifi AC LR Access Point