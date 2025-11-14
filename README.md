Ansible_For_Network

Multi-Vendor Network Automation with Ansible 2.9.9

This repository provides hands-on automation examples for multiple network vendors using Ansible 2.9.9.
Each vendor folder contains playbooks, inventory examples, and configuration templates to help engineers learn and automate real-world scenarios across different platforms.

📁 Repository Structure
Ansible_For_Network/
│
├── Project_Cisco_Learning/
│   └── (Playbooks, inventory, templates)
│
├── Project_Fortinet_Learning/
│   └── (Playbooks, inventory, templates)
│
├── Project_Huawei_Learning/
│   └── (Playbooks, inventory, templates)
│
├── Project_Juniper_Learning/
│   └── (Playbooks, inventory, templates)
│
├── Project_Nokia_Learning/
│   └── (Playbooks, inventory, templates)
│
└── README.md

🌐 Supported Vendors & Versions

This project includes automation examples for the following network systems:
Vendor	Platform / OS version	Notes
Cisco	IOS-XE	Routing, interfaces, VLANs, OSPF, BGP
Nokia	TiMOS-B-12.0.R6	SR-OS basic automation, L2/L3 services
Huawei	NE40 Series	Interfaces, OSPF, BGP, basic provisioning
Juniper	vMX 22.01 automation.
Fortinet	FortiOS v7.0.3 Build0237	Firewall policies, interfaces, objects

🛠 Requirements
Software
Ansible 2.9.9
Python 3.x
SSH connectivity (for IOS-XE, Huawei, Nokia, Juniper)
API or SSH for Fortigate
Python Dependencies

Install from your own requirements file or simply:
pip install ansible==2.9.9 paramiko netmiko jinja2 requests

▶️ How to Run a Playbook
The command structure used in this project follows this format (as shown in the diagram below):
ansible-playbook -i hosts Playbook_deploy_interfaces.yaml

Breakdown:
ansible-playbook → command to run a playbook
-i hosts → inventory file containing device IPs
Playbook_deploy_interfaces.yaml → your automation logic

2. Ansible Execution Diagram

Helps beginners understand how to run playbooks:

ansible-playbook   -i   hosts   Playbook_deploy_interfaces.yaml
     |             |      |                 |
  Command      Inventory  Host file     Name of the playbook

🚀 What You Can Learn From This Project
🔹 Cisco IOS-XE

Configure interfaces
Deploy routing protocols (OSPF, BGP)

Automate VLANs, ACLs

Gather device facts

🔹 Nokia SR-OS (TiMOS 12.0.R6)
Configure router interfaces
Automate L2/L3 services
Retrieve system, chassis, and routing information

🔹 Huawei NE40
Interface provisioning
Routing (OSPF/BGP)
NETCONF/YANG automation (if enabled)

🔹 Juniper vMX 22.01
NETCONF operations
Commit scripts
Routing configuration templates

🔹 Fortinet FortiOS
Firewall rules automation
Interface configuration
Security objects
Address groups & Address objects

📘 Purpose of the Project
This repository is designed for:
Network engineers learning automation
Preparing for NetDevOps roles
Multi-vendor automation training
Lab testing and demonstrations
Building real-world reusable automation templates
It covers all major vendors used in modern service providers and enterprise networks.

🧩 Future Enhancements
Planned improvements include:
Adding dynamic inventory examples
Full CI/CD integration (GitHub Actions)
NETCONF/YANG examples (Huawei, Nokia, Juniper)

API automation (Fortigate, Cisco RESTCONF)
