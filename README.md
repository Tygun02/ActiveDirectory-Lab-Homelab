 # Active Directory Homelab (Windows Server)

# 🧩 Active Directory Homelab Portfolio

This project showcases my hands-on experience setting up and managing an **Active Directory (AD) environment** in a virtualized lab.  
It was built from scratch on **VMware Workstation** using a **Dell laptop** running Windows, and includes PowerShell automation for user and group management.

---

## 🎯 Objectives

The goal of this lab was to demonstrate my ability to:
- Deploy and configure a **Windows Server domain controller**
- Join Windows clients to a domain
- Configure and manage **Group Policy Objects (GPOs)**
- Set up and manage **DNS, DHCP**, and file sharing services
- Automate administrative tasks using **PowerShell**
- Simulate a small-scale enterprise network environment for training and troubleshooting

---

## 🧱 Lab Architecture

| Role | Hostname | OS | Description |
|------|-----------|----|-------------|
| Domain Controller | DC01 | Windows Server 2022 | AD DS, DNS, DHCP |
| Windows Client | CL01 | Windows 11 Pro | Joined to domain, used for testing GPOs |
| Optional Admin Machine | ADM01 | Windows 11 | Management and scripting workstation |


---

## 📌 Key Highlights
- ⚙️ Built a **Windows Server 2022 VM** and promoted it to a **Domain Controller**
- 🌐 Configured **DNS and networking** for domain services
- 🗂️ Designed a structured **OU hierarchy** (IT, HR, Sales)
- 👥 Automated **user and group creation** with PowerShell
- 🔒 Applied **Group Policy Objects (GPOs)** for password complexity & security baselines
- 📑 Exported **GPO reports and backups** for documentation

---

## 📄 Portfolio Downloads
- 📘 [Full Portfolio (with Screenshots)](docs/ActiveDirectory-Homelab-Portfolio.pdf)  
- ⚡ [Executive Summary (1-page overview)](docs/ActiveDirectoryHomelab-Summary.pdf)

---

## 🌐 Live Site
You can also view the project portfolio online via **GitHub Pages**:  
👉 [Live Project Walkthrough](https://tygun02.github.io/ActiveDirectory-Lab-Homelab/)

---

## 📂 Repository Structure
- `docs/` → GitHub Pages site (`index.md`, images, PDFs)  
- `scripts/` → PowerShell automation scripts  
- `README.md` → This file  

---

👤 **Author:** Kingsley Otoo  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/kingsley-otoo-6aabb0273)  
