# Linux Security Hardening Lab

## Overview

This project demonstrates a basic Linux security assessment and hardening process performed on a Kali Linux virtual machine.

The objective was to evaluate the system's security posture, identify potential attack surface exposure, and implement security improvements to reduce risk.

---

## Objectives

* Review privileged user accounts
* Identify running services
* Verify open network ports
* Assess SSH configuration
* Install and configure a firewall
* Reduce the system attack surface

---

## Tools Used

* Kali Linux
* UFW (Uncomplicated Firewall)
* systemctl
* ss
* grep

---

## Assessment Activities

### 1. Privileged User Review

Verified local administrative accounts and confirmed that only the authorized user belonged to the sudo group.

### 2. Running Services Review

Enumerated active system services to identify unnecessary or potentially exposed services.

### 3. Network Exposure Assessment

Reviewed listening TCP and UDP ports using Linux networking tools.

Result:

* No listening network services were identified.

### 4. Firewall Hardening

Installed and configured UFW firewall.

Configuration applied:

* Default deny incoming connections
* Default allow outgoing connections
* Firewall enabled and verified

### 5. SSH Security Review

Verified that:

* SSH service was installed
* SSH service was not running
* SSH automatic startup was disabled

---

## Findings

* Only one privileged user account was identified.
* No unnecessary listening ports were exposed.
* UFW firewall was successfully configured.
* SSH was not exposed to the network.
* The overall attack surface was reduced.

---

## Screenshots

### Running Services Review And Network Exposure Assessment

![Running Services](screenshots/running-services-and-open-ports.png)

### Firewall Configuration

![Firewall Status](screenshots/firewall-status.png)

### SSH Service Review

![SSH Service Status](screenshots/ssh-service-status.png)

### SSH Startup Status

![SSH Disabled](screenshots/ssh-disabled.png)

---

## Skills Demonstrated

* Linux Administration
* Linux Security
* Firewall Configuration
* Service Enumeration
* Security Hardening
* Network Security Fundamentals
* Security Assessment
