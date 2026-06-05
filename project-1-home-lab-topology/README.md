# Project 1 — Home Lab Topology

## Overview
A simulated enterprise network built in EVE-NG using Mikrotik RouterOS.
Demonstrates basic routing, IP addressing, and network segmentation.

## Network Diagram
VPC3 (10.0.1.10) --- Mikrotik1 --- Mikrotik2 --- VPC4 (10.0.3.10)
10.0.1.1   10.0.2.1/10.0.2.2   10.0.3.1

## IP Address Table
| Device | Interface | IP Address |
|--------|-----------|------------|
| VPC3 | eth0 | 10.0.1.10/24 |
| Mikrotik1 | ether1 | 10.0.1.1/24 |
| Mikrotik1 | ether2 | 10.0.2.1/24 |
| Mikrotik2 | ether1 | 10.0.2.2/24 |
| Mikrotik2 | ether2 | 10.0.3.1/24 |
| VPC4 | eth0 | 10.0.3.10/24 |

## What I Built
- Configured IP addresses on router interfaces
- Built static routing tables so traffic forwards correctly between segments
- Verified end-to-end connectivity with ping (TTL=62 confirming 2 router hops)

## Tools Used
- EVE-NG Community Edition
- Mikrotik RouterOS CHR 7.1
- VPCS (Virtual PC Simulator)

## Key Concepts Demonstrated
- IP subnetting and addressing
- Static routing
- Network segmentation
- TTL and hop counting
