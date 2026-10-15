# Secure Digital Payments Network

A Cisco Packet Tracer simulation demonstrating network connectivity, dynamic routing, and access control in a digital-payments environment.

## Overview

This project simulates a digital payments network connecting a customer, merchant, payment gateway, and two bank networks. It demonstrates communication between different networks and the use of access control policies to restrict unauthorized direct access to selected bank networks.

## Network Components

- **Customer Network:** Represents the customer-side network.
- **Merchant Network:** Represents the merchant-side network.
- **Payment Gateway:** Hosts a sample payment gateway webpage.
- **Bank A and Bank B:** Represent separate banking networks with sample ledger webpages.
- **DNS Server:** Resolves the `pay.local` domain to the payment gateway server.
- **Syslog Server:** Demonstrates remote logging of network events.

## Key Features

- Multi-router network topology
- OSPF dynamic routing
- Extended Access Control Lists (ACLs)
- IPv4 addressing and subnetting
- DNS and HTTP/HTTPS services
- Sample banking ledger webpages
- Packet Simulation Mode testing
- Remote Syslog demonstration

## Technologies Used

- Cisco Packet Tracer
- OSPF
- IPv4
- Extended ACLs
- DNS
- HTTP/HTTPS
- Syslog

## Security Demonstration

The project demonstrates network-level traffic restrictions using router ACLs.

| Test Scenario | Expected Result |
|---|---|
| Customer PC to Payment Gateway | Allowed |
| Customer network to Bank A network | Blocked |
| Customer network to Bank B network | Blocked |
| Bank A network to Bank B network | Blocked |

These tests demonstrate configured connectivity and access-control policies in the simulated network.

## How to Run

1. Download the `.pkt` file from this repository.
2. Open it using Cisco Packet Tracer.
3. Inspect the network topology and router configurations.
4. Use the CLI to examine OSPF and ACL configurations.
5. Switch to Simulation Mode to observe packet delivery and access restrictions.

## Project Limitations

This project simulates network infrastructure for a digital-payments environment. It does not implement actual money transfers or a live payment-processing application. The banking ledger webpages contain sample static records and do not connect to a live database. Customer authentication and automatic payment processing are outside the current implementation.
