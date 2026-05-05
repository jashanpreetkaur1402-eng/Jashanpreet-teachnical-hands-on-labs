# Lab 2: Active Directory & Domain Controller Configuration

##  Project Overview
This lab demonstrates the configuration of a Windows Server environment into a functional Active Directory forest. It involves promoting a primary server to a Domain Controller and adding a secondary server for high availability and redundancy.

 Lab Requirements
* **Domain Name:** `rogers-858.ca`
* **Primary DC (KAM-1-858):** * Static IP: `172.20.1.1` 
  * Roles: ADDS, DNS (Global Catalog)
* **Secondary DC (DOT-2-858):** * Static IP: `172.20.1.5`
  * Role: Secondary Domain Controller

##  Tasks Completed
* **Network Foundation:** Configured static IPv4 addresses and established DNS loops to allow for domain communication.
* **Forest Deployment:** Promoted the first server to the root of a new forest using the Active Directory Domain Services (ADDS) wizard.
* **Domain Redundancy:** Successfully joined the second server to the `rogers-858.ca` domain and promoted it as an additional Domain Controller.
* **Connectivity:** Enabled Network Discovery and File Sharing to allow cross-server resource management.

##  Verification
Verified the deployment using the **Active Directory Users and Computers (ADUC)** tool, ensuring both servers were correctly registered in the "Domain Controllers" container and replicating properly.

## Lab Evidence
<img width="711" height="418" alt="image" src="https://github.com/user-attachments/assets/f4579279-ad57-4972-8901-89487ea613eb" />


