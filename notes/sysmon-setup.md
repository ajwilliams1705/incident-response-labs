# Sysmon Setup - Windows SOC Lab

## Purpose
Familiarize myself with the Sysmon installation process. Sysmon is a tool that provides detailed information about processes for incident detection  and investigation

## Environment
- OS: Windows 10 (VirtualBox VM)
- Role: SOC / Incident Response Lab Endpoint
- Hypervisor: VirtualBox

## Installation
Sysmon was installed using the official Sysinternals binary and a community configuration[SwiftOnSecurity](https://github.com/SwiftOnSecurity/sysmon-config)


Command used: sysmon.exe -accepteula -i sysmonconfig-export.xml

## Configuration Source
- SwiftOnSecurity Sysmon configuration
- Focused on process creation, network connections, file creation, registry changes, and DNS queries.

## Key Event IDs Observed
- Event ID 1 – Process Creation
- Event ID 3 – Network Connection
- Event ID 11 – File Creation
- Event ID 13 – Registry Value Set
- Event ID 22 – DNS Query

## Verification
Sysmon events were confirmed in:
Event Viewer → Applications and Services Logs → Microsoft → Windows → Sysmon → Operational

## Snapshot
A VirtualBox snapshot was taken after successful installation:
"Windows + Sysmon (SOC Baseline)"
