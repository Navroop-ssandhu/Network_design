### Tech Solutions Inc. Network Infrastructure Design ###

This project provides a detailed network infrastructure design for Tech Solutions Inc., a medium-sized IT consulting firm with approximately 200 employees across various departments. The design incorporates advanced networking solutions tailored for each department’s unique requirements, emphasizing security, organization, and scalability. Special attention has been given to cable management, Intermediate Distribution Frame (IDF) and Main Distribution Frame (MDF) placements, device selection, and cost-effectiveness.

## File Structure

This repository includes the following files:

1. GROUP-C.pdf: PDF version of the network diagram, useful for easy viewing and sharing.

2. GROUP-C.png: PNG image of the network diagram for quick reference and visualization.

3. GROUP-C.vsdx: Original Visio file used to create the network diagram, which can be edited for future modifications.

4. ReadMe.txt: Text file with additional information or instructions related to the project.

5. Scenario.txt: Contains the project scenario and requirements, providing context for the design decisions.

## Project Overview
Tech Solutions Inc. operates across two floors with five primary departments: HR, Sales, IT Support, Development, and Research & Development (R&D). Each department’s network configuration reflects its specific operational needs, including VLAN segmentation, dedicated network devices, and tailored access controls. This design also includes additional devices to enhance network robustness, secure data handling, and effective traffic management.

## Key Design Focuses:

1. Departmental Differentiation and Customization:
Each department is visually and functionally distinguished using VLAN assignments and unique subnets, as well as labeled equipment. These configurations ensure isolated and secure traffic flows within and between departments.

2. Cable Management:
All connections follow a structured cable management protocol to enhance maintenance efficiency and reduce clutter. Cable pathways are carefully mapped to connect each department’s IDF with the core switch located in the MDF.

3. IDF & MDF Placements:
MDF (Main Distribution Frame) is centrally located to connect core network components, including the core switch, firewall, and internet gateway.
IDFs (Intermediate Distribution Frames) are strategically placed within each department to minimize cable lengths and enhance network performance. IDFs also support departmental switches and routers to reduce latency and increase accessibility for maintenance.

4. Network Devices:
The network includes additional switches and routers to ensure redundancy and handle the specific needs of each department. High-performance core and access switches are used to maintain stable connections across all devices.
Firewall and NAT (Network Address Translation) setup are implemented at the internet gateway to secure external connections and translate public IP addresses to private ones within the network.

5. Cost Management:
The design considers cost-effective solutions without compromising quality. Devices were selected based on performance and scalability to optimize the balance between upfront investment and long-term maintenance costs.

6. Security and Access Control:
VLANs and Access Control Lists (ACLs) are configured to segregate departmental traffic and protect sensitive information. The firewall also acts as an added security layer at the internet gateway to prevent unauthorized access.


## Departments and Their Requirements

1. HR Department
Employees: 20
Requirements: Secure access to employee records, payroll systems, and intranet.
Devices: 1 HR server, 1 switch, 1 router, 5 PCs, 1 NAS for file storage.
VLAN: 50 – Isolated for access control to sensitive HR data.

2. Sales Department
Employees: 50
Requirements: Access to CRM software, internet, and a shared presentation server.
Devices: 1 Sales server, 2 switches, 1 router, 25 PCs, 2 IP phones, and a Network Attached Storage (NAS) device for CRM data.
VLAN: 10 – Segregated for secure CRM access and file sharing.

3. IT Support Department
Employees: 30
Requirements: Access to ticketing systems, remote management tools, and a database server.
Devices: 1 IT support server, 1 switch, 1 router, 15 PCs, 1 backup server.
VLAN: 20 – Isolated to support internal IT operations and troubleshooting.

4. Development Department
Employees: 100
Requirements: Access to development servers, version control systems, and testing environments.
Devices: 2 Development servers, 3 switches, 1 router, 50 PCs, 2 virtual servers for testing.
VLAN: 40 – Segregated to allow safe access to development environments and testing platforms.

5. Research and Development (R&D) Department
Employees: 30
Requirements: Secure access to research databases and collaboration tools.
Devices: 1 R&D server, 1 switch, 1 router, 10 PCs, 1 NAS for research data storage.
VLAN: 30 – Provides secure, isolated access for sensitive research and development data.

## Network Infrastructure
The infrastructure layout is designed with a central MDF connected to departmental IDFs. Core and access switches are deployed to support high-speed, reliable connections across the network, while firewalls and VLANs ensure that each department’s data remains secure and accessible only to authorized personnel.


=> Key Components:

1. Core Switch (CORE-SW-5P) – Acts as the central hub, connecting all departments and providing high-speed data handling capabilities.

2. Departmental Routers and Switches – Dedicated routers and switches for each department to handle traffic, segregate data, and ensure reliable access.

3. Firewall – Located at the internet gateway for external security, managing incoming/outgoing traffic through NAT.

4. Wireless Access Points – Placed strategically to provide wireless coverage across the office, ensuring smooth connectivity for mobile devices.

=> Additional Devices and Justifications
1. NAS (Network Attached Storage) – Dedicated NAS devices are placed in departments requiring high-volume data storage (Sales, R&D) to manage files securely and enhance accessibility.

2. Virtual Servers – Used in the Development department for testing environments, adding flexibility for project development and deployment without impacting the main servers.

3. IP Phones – Deployed in the Sales department, providing direct VoIP access, which is crucial for customer interactions and communications.

## VLAN Configuration

Each department operates on a distinct VLAN, with traffic segmentation to provide:
1. Enhanced security

2. Improved network performance

3. Isolated access to department-specific resources


## Network Diagram

The network diagram (see GROUP-C.png/HTML Document) illustrates the complete infrastructure layout:

1. Cable Management: Shows organized cable paths from IDFs to the MDF.

2. VLAN Labels and Color Codes: Different colors are used to represent each VLAN, making it easy to identify department boundaries.

3. Device Placement: Clearly labeled routers, switches, NAS devices, servers, and WAPs are placed within departmental boundaries for easy visualization.