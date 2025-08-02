# 💼 Firewall & VPN Administration Lab – Step 1: Azure Network Architecture

## 🔹 Project Overview

This is the first phase of my Firewall & VPN Administration Lab project. In this step, I designed and deployed a segmented network environment in Microsoft Azure to simulate an enterprise-grade foundation for VPN and firewall testing.

---

## 🔧 What I Did

- Created a **Virtual Network (VNet)** named `SecureRemoteVNet` with a `10.0.0.0/16` address space
<img width="1251" height="853" alt="Screenshot 2025-08-02 at 12 51 06 PM" src="https://github.com/user-attachments/assets/0acd8cc5-a54d-468e-9f4a-500dc9389118" />

  
- Designed and implemented the following **subnets**:
  - `VPN-Subnet` – `10.0.1.0/24` → for hosting OpenVPN CE
  - `Internal-Subnet` – `10.0.2.0/24` → for internal Linux/Windows test servers
  - `Remote-Users` – `10.0.3.0/24` → to simulate remote worker access
<img width="1447" height="823" alt="Subnets" src="https://github.com/user-attachments/assets/09c0d072-2be5-40a9-86cd-7cd035bee31d" />

    
- Prepared for secure access control by associating **Network Security Groups (NSGs)** to each subnet
<img width="1242" height="861" alt="NSGs" src="https://github.com/user-attachments/assets/9f7b435e-8e77-455f-9de5-5163856af12a" />

  

---

## 🛠️ Tools & Services Used

- Microsoft Azure Portal
- Virtual Network & Subnets
- IPv4 CIDR planning
- Network Security Groups (NSG)

---

## 🧠 Purpose

This network architecture is designed to support future phases of the project including:
- Remote access via VPN
- Firewall configuration
- Internal resource isolation
- Segmentation testing

It follows security best practices like **least privilege** and **network segmentation** used in real-world corporate environments.

---

## 📸 Network Diagram

![Azure VNet](https://github.com/user-attachments/assets/d4f77739-df0b-48ba-b091-c890921b4582)


---

## 🚀 Next Phase

In **Step 2**, I will deploy and configure an OpenVPN server in the VPN subnet to enable secure remote access to internal network resources.

Stay tuned!
