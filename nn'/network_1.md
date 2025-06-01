# Network Design
This section gives the detailed network design.

 [Assumptions](#assumptions) 

 [Network Design Diagrams and Justifications](#network-design-diagrams-and-justifications) 

 [WiFi Design](#wifi-design) 

 [Address Allocations](#address-allocations) 

 [Recommended Hardware](#recommended-hardware) |

## Task 4.1.1: Assumptions

THe following are the assumptions made
- location of headquaters - Melbourne CBD (Main office and Data centre)
- locatio of 3 branches - Essendon fields, Dandenong and Derimutt 
- Number of staff in Headquaters - 70
- Number of staff in Essendon Fields Headquaters - 30

## Task 4.1.2 Design the Network 

**1. Network Diagrams**
The following is the High level Design for WAN connectivity between branches and Head Quarters
![WAN Connectivity Network Diagram](images/WAN-connectivity.png) 

The following is the Head Quarters Network Diagarm
![Head Quarters Network Diagram](images/Head-Quarters-Network-Diagram.png) 

The following is the Essendon Fields Branch Network Diagarm
![Branch Network Diagram](images/Essendo-Fields-Network-Diagram.png) 

**2. Key Design Decisions**
1. Primary and Secondary WAN links at each site for redundacy purposes
2. Palo-Alto Firewalls for traffic control and VPN users 
3. SD-wan devices for layer 3 routing at each site, assumping headquaters work as a hub and all the other branch devices work as spokes, they also act as firewalls at branch sites. 
4. On-prem and cloud hosted redudant servers are built, taking further improvement, load balancing and public access into consideration


**3. WiFi Design**

The following is the Wi-Fi Design which depicts Essendon fields Wifi Design

![Branch Wi-Fi Design Diagram](images/Branch-Wifi-Design.png)

The following Design depicts the SSID segementation 

![Wi-Fi SSID Design Diagram](images/Wi-Fi-SSID-Design.png)

THe following are the design parameters used on Access-points 

- Encryption method: WPA2 with AES (Advanced Encryption Standard

- Wi-Fi Standards: 802.11ax 

- Frequency Bands: 2.4 Ghz, 5Ghz and 6 Ghz 

- The following SSID's are used so users of different platofrms can connect to appropriate Wi-Fi SSID's

   1. Corporate Network - Travel Agency Employess will connect to this Wifi System with their Employee login details 
   2. Guest Network -  External vendors and guests connect to this Wifi system (password will be shared by Employees) 
   3. Iot Network - For Scanners and any Iot related devices 

**4. Address Allocations**

The following are the IP subnets used 
/16 subnet - 42.50.0.0/16 (42 is the last two digits of surya's student ID)
where /16 will be further divided into /24 subnets for specific segmentaions like branches, Wifi, servers, CCTV, wired Data, IOT devices, sensors and scanners. 
The following is the IPsubnetting Diagram that depicts the use of IP subnetting at Headquarters and Essendon field branch office 
![IP-SUbnetting Design Diagram](images/IPsubnetting.png)

**5. Recommended Hardware**

firewalls:
 - Company: Palo-Alto 
 - Model: PAN-PA-5450
 - Cost: AUD $157,703.18
 - Website: https://www.router-switch.com/paloalto-pan-pa-5450.html
Layer 3 Routers:
 - Company: Velocloud 
 - Model: 740 500 Mbps series for Headquaters and 720 200 Mbps series for Branches 
 - Cost AUD $ 16,00
 - Website: https://www.broadcom.com/products/software/velocloud-sd-wan
Switches: 
 - Company: HP  
 - Model:  Aruba 6300M Core switches and Aruba 6200F 24 port series as access switches
 - Cost: $25,024.00 and $4,596.00
 - Website: https://www.pclan.com.au/products/hpe-aruba-6300m-24-port-24x10g-sfp-4x50g-sfp56-manageable-switch?_pos=1&_psq=JL658A&_ss=e&_v=1.0
   https://www.pclan.com.au/products/hpe-aruba-6200f-24-port-4x10g-sfp-poe-370w-manageable-gigabit-switch?srsltid=AfmBOorC0scCPx8g9LGKC1k1W5ipZMF6m8GhoGZqiK9U4rop00xpdz74
Wi-Fi Access Points:  
 - Company: Meraki 
 - Model: MR36H
 - Cost AUD $840.61
 - Website: https://www.buymeraki.com.au/meraki-mr36h-hw-meraki-mr36h-wi-fi-6-cloud-managed-ap/?srsltid=AfmBOor1twMXGWM8YBFl_QyD5pNBpSDmEwhZFlLG_uLJs3yGHwd4RIBF



