# Interview Guide — Zero Trust Healthcare Architecture

## 30-Second Explanation
My capstone designed a Zero Trust-oriented network architecture for a 1,500-user healthcare organization. I divided the environment into nine VLAN security zones and documented firewall policy, vendor VPN/MFA access, DMZ design, monitoring, risk analysis and AWS/Azure integration. The main objective was to reduce lateral movement while still allowing required clinical and business communication.

## Questions I Can Discuss
- Why I selected nine VLAN zones.
- How segmentation limits lateral movement.
- How a vendor should reach an approved application without broad internal access.
- Why guest Wi-Fi must remain separated from corporate resources.
- How firewall rules implement least privilege between zones.
- Why monitoring remains necessary after segmentation.
- How cloud networks fit into an enterprise security architecture.
- How the design maps to Zero Trust principles.

## Design Principle
**Do not trust traffic because of where it originates. Verify identity and access requirements, minimize reachable resources, and monitor important activity.**
