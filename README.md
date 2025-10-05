# Configuring-and-Testing-VLANs-
This project focuses on configuring and testing Virtual Local Area Networks (VLANs) to demonstrate how network segmentation enhances traffic management, security, and performance within an enterprise environment. The setup was implemented using a multilayer switch, a router, and two end-user PCs in Cisco Packet Tracer.

The main objective was to create and configure three VLANs — VLAN 10 (IT Department), VLAN 20 (HR Department), and VLAN 30 (Finance Department). Each VLAN was assigned a unique IP subnet to isolate broadcast domains and improve data flow control:

VLAN 10 – 10.16.8.1/24

VLAN 20 – 10.16.10.1/24

VLAN 30 – 10.16.12.1/23

After creating and naming the VLANs, the appropriate switch ports were assigned to each VLAN (VLAN 10 → ports 1–2, VLAN 20 → ports 3–4). The PCs were connected to ports under VLAN 10 and configured with IP addresses from the corresponding subnet (e.g., 10.16.8.2 and 10.16.8.3).

To verify connectivity, a continuous ICMP echo test (ping -t) was initiated between the two PCs. Successful replies confirmed proper VLAN configuration and intra-VLAN communication. When one PC was moved to a port under VLAN 20, the ping failed — demonstrating that devices on separate VLANs cannot communicate without inter-VLAN routing.

This experiment highlights the importance of VLANs in enterprise networks, particularly in terms of traffic segmentation, security, and broadcast control. It also reinforces the role of a multilayer switch or router-on-a-stick configuration in enabling communication between VLANs.

Overall, this project provided hands-on experience in VLAN configuration, port assignment, IP addressing, and basic network troubleshooting using Cisco Packet Tracer. It serves as a foundational exercise for understanding Layer 2 segmentation and preparing for more advanced topics like inter-VLAN routing, trunking, and network security implementation.<img width="827" height="394" alt="LinkedIn topology" src="https://github.com/user-attachments/assets/f7f0f212-b7fb-4233-b257-54fcf1b13c4e" />
<img width="1447" height="522" alt="vlan 10" src="https://github.com/user-attachments/assets/f1544493-4702-4f56-b46d-9e7ce8d67f34" />
<img width="1311" height="502" alt="valn 20-30" src="https://github.com/user-attachments/assets/089ad431-da77-4e0d-a12f-9a7084054d74" />
<img width="1451" height="505" alt="vlan brief" src="https://github.com/user-attachments/assets/d6e44f1a-8de6-4633-a35b-43f66c71ee79" />
<img width="1448" height="496" alt="vlans int brief" src="https://github.com/user-attachments/assets/5d6530a9-5b41-45ba-a70f-97951fca5c58" />
<img width="1249" height="381" alt="ping 1" src="https://github.com/user-attachments/assets/1dc3dbff-e825-4149-9dfb-3af24f675c61" />
<img width="1356" height="417" alt="ping 2" src="https://github.com/user-attachments/assets/81bfd373-a195-41eb-814e-487017bf4904" />
