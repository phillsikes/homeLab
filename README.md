# homeLab

Hi there, I'm Phill and this is my homeLab. 

It's a work in progress, so check back later for more interesting projects and documentation.

## Goals
- Have a place to learn about and test technologies I'm interested in.
- Provide services for my family and friends.
- Study for certifications, currently GCP Cloud Engineer and RHCSA.

## Overview
My homeLab is in a constant state of motion. It's been through multiple iteration of network configurations and hardware, starting with a pfSense router and Meraki hardware (until the licence ran out), then to an OPNsense box and Unifi gear. At the moment my Home network runs off a set of Mesh APs segregated from the Lab network, which includes a dedicated router, switch and AP.

On the Lab network is a cluster of Raspberry Pi 5s set up with Kubernetes and monitoring for hosting services and learning. In addition there are Dell SFF boxes to test out and build interesting projects as I develop my homeLab.

I'll update this as time allows and plan to include some howTo articles in the future. 

## The Systems

### clusterPi

Primary Use: 
Setup to run K3s Lightweight Kubernetes to provide local services and stay up to date on current technologies and processes. 1 Master node and 2 Worker nodes set up to run services like WordPress and Pi-Hole, using Persistent Volumes, Horizontal Pod Autoscaling and monitoring. The Raspberry Pi hardware recieves the most support on Debian based platforms, so I chose to run Ubuntu Server as the primary OS for the cluster.

Hardware
- 3x Raspberry Pi 5 8GB
- 1.5TB NVMe SSD Storage

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
- 1TB NVMe SSD
- 512GB SSD
- Intel I350-T4 Quad Gigabit NIC

Software
- RHEL 10 Server w/ GUI
- Ghostty

## The Network

Hardware
- Unifi Cloud Gateway Ultra
- Unifi Switch 8 60W (8-Port Managed Gigabit Switch with PoE)
- Unifi AC LR Access Point

## Depreciated Gear
Monstro Workstation
- Apple Mac Pro Dual Xeon

Networking Gear
- Optiplex Firewall - OPNsense
- Netgate SG-2440 Firewall - pfSense
- Meraki-8P PoE Switch
- Meraki AP