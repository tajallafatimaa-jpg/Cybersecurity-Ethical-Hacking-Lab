# Cybersecurity-Ethical-Hacking-Lab

Practical cybersecurity lab environment using VirtualBox, Kali Linux, Windows VMs, NAT networking, IP configuration, connectivity testing, and VM snapshots.

# Cybersecurity & Ethical Hacking Lab Environment

## Overview

This repository documents my hands-on setup of a practical Cybersecurity, Ethical Hacking, and Penetration Testing Lab Environment using virtual machines and VirtualBox.

The lab was created as an isolated environment for practicing cybersecurity concepts, network configuration, ethical hacking techniques, penetration testing, and future CTF-based exercises.

The setup follows a two-phase approach covering the installation and configuration of VirtualBox, Kali Linux, Windows virtual machines, network configuration, IP addressing, connectivity testing, and VM snapshots.

## Lab Objectives

- Build an isolated cybersecurity practice environment.
- Configure VirtualBox networking using a custom NAT Network.
- Install and configure Kali Linux.
- Configure Windows virtual machines for security testing.
- Assign and verify IP configurations.
- Test connectivity between virtual machines.
- Create VM snapshots for safe experimentation and rollback.
- Prepare the environment for future CTF and penetration-testing labs.

---

## Lab Environment & Specifications

### Virtualization

- **Hypervisor:** Oracle VirtualBox
- **Archive Utility:** 7-Zip
- **Virtual Machines:** Multiple Virtual Machines

### Operating Systems

- **Attacker OS:** Kali Linux
- **Target OS:** Windows 10/11/7
- **Android VM:** Optional

### Network

- **Network Type:** NAT Network
- **Network Subnet:** `10.0.0.0/24`
- **Configured IP Range:** `10.0.0.2` – `10.0.0.99`

---

## Network Topology

The general lab architecture is structured as follows:

```text
                 Host Machine
                     |
               VirtualBox
                     |
              NAT Network
             10.0.0.0/24
                     |
       +-------------+-------------+
       |             |             |
     Kali         Windows       Android
   Linux VM         VM            VM
       |             |             |
       +-------------+-------------+
              Connectivity Tests
