# Architecture Decisions

## 1. Segment by Trust and Function
The design separates users, servers, clinical systems, vendors, management, security tooling, wireless networks and the DMZ into distinct VLAN zones. The purpose is to reduce unnecessary lateral connectivity and make access rules explicit.

## 2. Isolate Third-Party Access
Vendor connectivity follows a controlled path using authentication, VPN access and firewall policy rather than placing third parties directly on trusted internal networks.

## 3. Protect Internet-Facing Services
Public-facing services belong in a DMZ so exposure of one service does not automatically provide unrestricted access to internal systems.

## 4. Apply Least Privilege
Firewall policy should permit required business flows rather than broad network-to-network access. Management and security-tool networks receive additional protection.

## 5. Centralize Visibility
SIEM, IDS/IPS and security logging concepts are included because segmentation without monitoring can limit movement but does not provide sufficient visibility into suspicious activity.

## 6. Treat Cloud as Part of the Architecture
AWS and Azure components are considered extensions of the enterprise security boundary. Identity, routing and access controls must remain consistent across on-premises and cloud environments.
