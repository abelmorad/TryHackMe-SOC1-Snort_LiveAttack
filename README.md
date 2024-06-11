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

- **Start Snort in sniffer mode and try to figure out the attack source, service, and port.**
  - In the CLI enter `snort -vde` to display the packet data, headers as well as the data link layer headers
  - Analyze the packet and look for anomalys
    - This IP keeps coming up in the packets
      - ![snortliveattack2](https://github.com/abelmorad/TryHackMe-SOC1-Snort_LiveAttack/assets/110463619/b22ebf3c-25c5-40ca-8a89-b2ae43e2cfeb)
    - It seems suspicious let us find out how many times this IP comes up. Enter snort -vde | grep 10.10.45.36
      - ![snortliveattack4](https://github.com/abelmorad/TryHackMe-SOC1-Snort_LiveAttack/assets/110463619/1cb8f16c-79a4-4598-b37b-1c6dc45d9e9a)



