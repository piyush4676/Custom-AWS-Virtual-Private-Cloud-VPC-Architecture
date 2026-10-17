# Custom AWS Virtual Private Cloud (VPC) Architecture

## 📋 Overview
This project demonstrates foundational cloud networking skills by designing a secure, isolated virtual network from scratch using Amazon VPC. Instead of relying on the default AWS VPC, this architecture establishes clear boundary layers separating public-facing components from private backend resources.

## 🏗️ Architecture & Network Design
1. **Custom VPC:** 
   * **CIDR Block:** `10.0.0.0/16` (Providing a pool of 65,536 private IP addresses).
2. **Subnet Segmentation (`/24` Subnet Masks):**
   * **Public Subnet (`project-subnet-public1-us-east-1a`):** Configured for resources that require direct access to the public internet (such as web servers or load balancers)[cite: 3].
   * **Private Subnet (`project-subnet-private1-us-east-1a`):** Isolated from direct internet exposure, ideal for secure backend databases and application logic[cite: 3].
3. **Internet Gateway (IGW):** Attached to the VPC to serve as a bridge between the public subnet and the external internet.
4. **Route Tables:** Configured distinct routing logic to direct internet-bound traffic from the public subnet through the Internet Gateway.

## 🛠️ Key Skills Demonstrated
* Designing cloud network topologies using CIDR blocks and subnet masking.
* Implementing network security isolation (Public vs. Private subnets).
* Configuring Internet Gateways and custom Route Tables.
* Reading and interpreting AWS VPC Resource Maps.

## 📸 Proof of Execution (VPC Resource Map)
# Custom AWS Virtual Private Cloud (VPC) Architecture

## 📋 Overview
This project demonstrates foundational cloud networking skills by designing a secure, isolated virtual network from scratch using Amazon VPC. Instead of relying on the default AWS VPC, this architecture establishes clear boundary layers separating public-facing components from private backend resources.

## 🏗️ Architecture & Network Design
1. **Custom VPC:** 
   * **CIDR Block:** `10.0.0.0/16` (Providing a pool of 65,536 private IP addresses).
2. **Subnet Segmentation (`/24` Subnet Masks):**
   * **Public Subnet (`project-subnet-public1-us-east-1a`):** Configured for resources that require direct access to the public internet (such as web servers or load balancers)[cite: 3].
   * **Private Subnet (`project-subnet-private1-us-east-1a`):** Isolated from direct internet exposure, ideal for secure backend databases and application logic[cite: 3].
3. **Internet Gateway (IGW):** Attached to the VPC to serve as a bridge between the public subnet and the external internet.
4. **Route Tables:** Configured distinct routing logic to direct internet-bound traffic from the public subnet through the Internet Gateway.

## 🛠️ Key Skills Demonstrated
* Designing cloud network topologies using CIDR blocks and subnet masking.
* Implementing network security isolation (Public vs. Private subnets).
* Configuring Internet Gateways and custom Route Tables.
* Reading and interpreting AWS VPC Resource Maps.

## 📸 Proof of Execution (VPC Resource Map)
<img width="1920" height="1080" alt="Screenshot (3514)" src="https://github.com/user-attachments/assets/f48e1cfa-834b-4f7a-b231-0efe0b244c0b" />

!<img width="1920" height="1080" alt="Screenshot (3515)" src="https://github.com/user-attachments/assets/70e26929-e8d9-4266-952d-bedf81cfaf43" />
