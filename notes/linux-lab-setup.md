
# Linux SOC Lab Setup

## Purpose
This document records the setup of a Linux virtual machine used for security operations support tasks such as traffic analysis, log review, and tooling.

The system is intended to complement the Windows endpoint during incident response labs.

## Environment
- OS: Ubuntu 22.04 LTS
- Role: SOC / Incident Response Lab Endpoint
- Hypervisor: VirtualBox
  
## Rationale for LTS
Ubuntu LTS was selected to ensure:
- Tool stability
- Long-term support
- Compatibility with common SOC tooling and tutorials

## Initial Setup
System was updated immediately after installation:

sudo apt update && sudo apt upgrade -y

## Installed tools
The following tools were installed
- Curl/ wget
- git
- tcpdump
- wireshark
- dnsutils
- python3

## Verification
Installed tools were verified by checking version output:

curl --version
git --version
python3 --version
tcpdump --version

## Snapshot
A VirtualBox snapshot was taken after successful installation: "Ubuntu SOC Lab (Baseline Tools Installed)."
