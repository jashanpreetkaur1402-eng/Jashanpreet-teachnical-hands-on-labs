# Lab 3: Active Directory Objects, Client Integration & Administration

## Project Overview
This lab covers the end-to-end lifecycle of Active Directory management. This includes designing an Organizational Unit (OU) hierarchy, provisioning users/groups, joining a Windows 10 client to the domain, and performing critical administrative maintenance tasks.

##  Phase 1: Directory Structure & Objects
I implemented the following departmental structure within the `rogers-858.ca` domain:

| Organizational Unit |                              Security Groups |                               User Provisioning |
| **Finance-858** |                                  Finance-Mgr, Finance-Staff |                  5 Real-name users |
| **Human-Resources-858** |                      HR-Mgr, HR-Staff |                                 5 Real-name users |
| **Information-Technology-858** |                    IT-Mgr, IT-Staff |                             5 Real-name users |

* **Logic:** Users were nested into Staff groups for baseline access, with one user per OU elevated to the Manager group for administrative testing.


##  Phase 2: Client Workstation Configuration (PC-3-858)
To integrate the Windows 10 workstation into the production environment, the following steps were completed:

* **Static Networking:**
    * **IP Address:** `172.20.1.100`
    * **Subnet Mask:** `255.255.255.0`
    * **Default Gateway:** `172.20.1.254`
    * **Preferred DNS:** `172.20.1.1` (KAM-1-858)
* **Domain Integration:** Successfully joined the `rogers-858.ca` domain and verified the connection via a Domain Administrator login.
* **Optimization:** Enabled Network Discovery and File Sharing for resource access.

---

##  Phase 3: Administrative Maintenance & Testing
I performed the following "Day 2" administrative tasks to verify domain health:
1.  **Replication Verification:** Confirmed synchronization between `KAM-1-858` and `DOT-2-858`.
2.  **User Lifecycle Management:** Tested account disabling and user account deletion.
3.  **Password Security:** Successfully implemented "Change password on next login" and performed manual password resets.
4.  **Remote Login:** Verified that new domain users could successfully authenticate onto the PC-3 workstation.


lab evidence 
Add all users to the Staff groups 
<img width="975" height="747" alt="image" src="https://github.com/user-attachments/assets/5ed16e9b-a1b1-4743-b276-ba0508555614" />
Successfully joined the `rogers-858.ca` domain and verified the connection via a Domain Administrator login
<img width="975" height="744" alt="image" src="https://github.com/user-attachments/assets/3bdd1c12-a815-4954-b96b-9f533111a6f1" />
<img width="970" height="694" alt="image" src="https://github.com/user-attachments/assets/e4270c29-4021-4a0a-abec-fe8e25b0bca0" />
<img width="975" height="813" alt="image" src="https://github.com/user-attachments/assets/a4eff0d4-e36e-4538-bddd-439325cefbb1" />
<img width="975" height="691" alt="image" src="https://github.com/user-attachments/assets/5012e88f-b44b-4126-925c-98d930e26c1f" />
<img width="975" height="459" alt="image" src="https://github.com/user-attachments/assets/4cd8ad1d-e299-44e8-be49-c9d3134ce76b" />
<img width="966" height="686" alt="image" src="https://github.com/user-attachments/assets/fe7ef194-baa1-4719-8988-cb04dca42d3a" />
<img width="783" height="478" alt="image" src="https://github.com/user-attachments/assets/4a1a691a-169f-4871-8717-7e6d160faf9b" />
<img width="963" height="677" alt="image" src="https://github.com/user-attachments/assets/157bcc26-0044-4fad-977e-daac12b064a2" />
<img width="944" height="673" alt="image" src="https://github.com/user-attachments/assets/122e8f42-8155-4560-b8b0-2590f7475e9d" />
