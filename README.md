# Documentation: TryHackMe SOC L1 - Snort Live Attack Challenge - Brute-Force

## 1. Introduction

- The room invites you to a challenge where you will investigate a series of traffic data and stop malicious activity work with Snort to analyze live and captured traffic
### Objective
- Observe the traffic with Snort and identify the anomaly first. Then you can create a rule to stop the brute-force attack and capture the flag

## 2. Setup 
### Prerequisites

- Basic knowledge of network security concepts
- Access to the TryHackMe platform

## 3. Procedures
### Brute-Force Scenario

- **Start Snort in sniffer mode and try to figure out the attack source, service, and port.**
  - In the CLI enter `snort -vde` to display the packet data, headers as well as the data link layer headers
  - **

