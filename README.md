# Milestone-Project

![NextGen Project](https://github.com/user-attachments/assets/fc48838a-96b1-47f3-b657-ba621f6c2158)




## Introduction

This project involved the successful planning and development of a comprehensive network system connecting a headquarters and its branch locations. The network infrastructure was designed to include routing, switching, voice over IP (VoIP), wireless connectivity, and robust security components. The primary objective was to ensure continuous connectivity, efficient data transmission, and secure communication across all branches, while optimizing network performance and safeguarding the integrity of the data being transmitted.

## HQ Configuration:

![HQ](https://github.com/user-attachments/assets/f849ec64-d1a1-4544-87c9-967485d50f69)

For the Headquarters building, two Cisco 3560 switches were installed and configured with advanced features including port-channel, Hot Standby Router Protocol (HSRP), Per VLAN Spanning Tree (PVST) with dual root configuration, split VLAN traffic, and a VTP server. Additionally, three Cisco 2960 Layer 2 access switches were installed to extend connectivity. A Cisco 2901 Router, equipped with IP Base and Security licenses, was installed as the primary internet router. This router serves as the primary firewall for internet access, providing Network Address Translation (NAT) and IOS-based firewalling for private subnets, including the guest network, acting as the company’s single internet exit point.

A Cisco 2911 router was deployed as the HQ WAN router, functioning as the gateway for all WAN services that connect the Headquarters to Branch 1 and Branch 2. This includes a private WAN connection to Branch 1 via a service provider, utilizing BGP peering. Additionally, a secondary internet service was connected to this router exclusively for establishing an IPSec Site-to-Site (L2L) VPN connection. Another Cisco 2911 router was installed as the HQ Voice Router, serving as the local call control for the Headquarters and Branch 2, as well as the PSTN Gateway for HQ. Wireless access points were installed to provide corporate network access via one SSID and guest network access via a separate SSID.

## Branch 1 Configuration:

![branch-1](https://github.com/user-attachments/assets/c9f5fdbd-8922-4cfc-88b6-9ee937e249bf)

A Cisco 2911 router was installed at Branch 1, serving as the gateway for connectivity to both the Headquarters and Branch 2 via the private WAN. This router also functions as the local call controller and PSTN gateway for Branch 1. Additionally, a wireless access point was installed, providing access exclusively to the corporate network.

## Branch 2 Configuration:

![branch-2](https://github.com/user-attachments/assets/6d4e4a32-a051-48cf-9413-348953a02e7f)

A Cisco 1941 router was installed at Branch 2, serving as the gateway for connectivity to the Headquarters and Branch 1 via a Site-to-Site VPN over the internet. This router ensures secure and reliable access between Branch 2 and the other locations.

## Conclusion

The successful implementation of this comprehensive network system across the Headquarters and branch locations has resulted in a robust and secure infrastructure that meets the organization’s operational needs. By deploying advanced routing, switching, and security technologies, the network ensures continuous connectivity, efficient data transmission, and secure communication. The integration of voice over IP, wireless access, and network segmentation further enhances performance and flexibility. This network is now well-positioned to support current demands and is scalable to accommodate future growth and technological advancements.
