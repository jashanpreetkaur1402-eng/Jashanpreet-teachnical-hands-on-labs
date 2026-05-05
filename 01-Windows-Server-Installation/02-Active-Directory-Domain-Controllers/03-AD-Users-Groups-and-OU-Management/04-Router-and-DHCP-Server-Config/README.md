# Lab 4: Router & DHCP Server Configuration

## Project Overview
This lab demonstrates the transition from static IP management to automated network infrastructure. The goal was to configure a Windows Server as a DHCP (Dynamic Host Configuration Protocol) server to dynamically assign IP addresses to clients within the `rogers-858.ca` domain.

##  Lab Requirements
* **DHCP Scope Name:** `Rogers-858-Scope`
* **Address Range:** `172.20.1.100` to `172.20.1.200`
* **Exclusions:** `172.20.1.1` to `172.20.1.20` (Reserved for Servers/Infrastructure)
* **Lease Duration:** 8 Days
* **Gateway/Router:** `172.20.1.254`

##  Tasks Completed
* **Role Installation:** Deployed the DHCP Server role on `KAM-1-858`.
* **Scope Configuration:** Defined the IP pool, subnet masks, and exclusion ranges to prevent IP conflicts with static servers.
* **Server Authorization:** Authorized the DHCP server within Active Directory to allow it to service client requests.
* **Client Testing (PC-3):** Reconfigured the Windows 10 client from a static IP to "Obtain an IP address automatically" and verified successful lease acquisition.
* **Reservation Management:** Demonstrated how to reserve a specific IP for a device based on its MAC address.

##  Verification
Verified the setup by running `ipconfig /all` on **PC-3-858**, confirming it received an IP from the `172.20.1.0` pool and identified `172.20.1.1` as its DNS server

###  Lab Evidence
 screenshot taken from the DHCP server, showing the ip range and the exclusion range of the dhcp scope.
<img width="756" height="486" alt="image" src="https://github.com/user-attachments/assets/77b8a9ee-9814-4af7-9d42-5eefbb985d23" />

showing the scope options (router and DNS)
<img width="758" height="442" alt="image" src="https://github.com/user-attachments/assets/9796348c-4b14-4eba-a67f-4a2b3d44f18c" />

screenshot taken from the DHCP server, showing that an ip address was leased to the client machine.
<img width="757" height="537" alt="image" src="https://github.com/user-attachments/assets/d29bb725-6970-4d26-9eaf-0f94b09845c3" />

after Configure PC-3 to obtain an IP automatically and verify the lease.
<img width="757" height="550" alt="image" src="https://github.com/user-attachments/assets/89cecbc9-2a73-4f18-aba5-9f270a34e8b7" />

screenshot taken from client machine showing the ip setting and a successful ping to 8.8.8.8.Test connectivity to external resources (like 8.8.8.8).
<img width="757" height="550" alt="image" src="https://github.com/user-attachments/assets/51eab7bc-93c4-4da5-971a-0d92a154d732" />

