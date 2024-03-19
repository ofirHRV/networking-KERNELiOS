
------------------------------ NETWORKING: FINAL PROJECT - KERNELIOS -------------------------------


course name:	Networking, KERNELiOS College for cyber-security
name:		Ofir Haruvi
grade: 		100

-----------------------------------------------------------------------------------------------------


The project is implemented as follows:

	**For detailed information about LANs and WANs, check the project file "networking exam.pkt".

1. VLANs:
	a. Division into VLANs - Subnetting:

		VLAN 10: 40 PCs			VLAN 50: 100 PCs
		VLAN 20: 12 PCs			VLAN 60: 50 PCs
		VLAN 30: 8 PCs			VLAN 70: 2 PCs
		VLAN 40: 4 PCs			VLAN 80: 2 PCs

		VLAN 90: 30 PCs			VLAN 130: 85 PCs
		VLAN 100: 30 PCs		VLAN 140: 40 PCs
		VLAN 110: 20 PCs		VLAN 150: 12 PCs
		VLAN 120: 15 PCs		VLAN 160: 3 PCs
		
				
		
		One computer is added to represent each VLAN.

	b. Implementation on the relevant switches (access & trunks).
	c. Implementation on the relevant routers using the "Router on a Stick" protocol.


2. WAN + Routing:
	a. Implementing networks between routers to create a WAN.

	b. Implementing routing protocols:

		* OSPF Between R1, R2, R3, R4, and multie-area OSPF between R3, R4, R6.
		* Default route (static) between routers R1, R2, R3, R4, R5, and floating route.


3. DHCP Protocol:

	a. Setting R1 as a DHCP Server.
	b. Creating a pool for VLAN 10 and VLAN 50 (remote network).


4. NAT Protocol:

	Implementing NAT in R4 for all VLANs towards network 192.168.5.0.


5. VTP + PVST Protocols:

	a. VTP for all VLANs with VTP server: SW1.
	b. PVST between SW1, SW2, SW3, SW4.


6. SSH Protocol:

	Enabling SSH on SW1.

	User: google
	Password: 123456


7. Port Security Protocol:

	Configuring port security on SW1, PC3 (VLAN 10).


8. Setting Passwords on a Switch:

	Setting passwords on SW1 for both User EXEC mode & Privileged EXEC mode: 123456.


9. ACLs:

	a. On R1: Only VLAN 10 won't be able to send ICMP packets to VLAN 140. Name: BLACKv10.
	b. On R2: Only PC 14 in VLAN 60 won't be able to communicate with 192.168.5.0/24. Name: BLACKpc14.


**