# Assignment 3 — Design a Three-Tier Network with Load Balancer on Azure

Part of the DevOps Micro Internship (DMI) with Agentic AI

---

## Purpose

In this assignment, you will create an Azure Virtual Network with separate web, application, and database subnets. You will deploy an Ubuntu VM running NGINX in the web subnet and make it accessible through a Public Load Balancer. The application and database subnets will remain empty.

---

# Task 1 — Create a Resource Group

## Goal

Create Resource Group `vnet-demo-rg` in Central India or your selected Azure region.

## Evidence

#### Screenshot 1 — Resource Group Overview showing `vnet-demo-rg` and its region

Add your screenshot here.

---

# Task 2 — Create a Virtual Network

## Goal

Create `eb-demo-vnet` (`10.0.0.0/16`) in `vnet-demo-rg` with `web-subnet` (`10.0.2.0/24`), `app-subnet` (`10.0.3.0/25`), and `db-subnet` (`10.0.4.0/26`). Azure Bastion is optional.

## Evidence

#### Screenshot 2 — VNet address space showing `eb-demo-vnet` uses `10.0.0.0/16`

Add your screenshot here.

---

#### Screenshot 3 — Subnets list showing the three required subnet names and CIDR ranges, including the Bastion subnet if applicable

Add your screenshot here.

---

# Task 3 — Create a VM in the Web Subnet

## Goal

Deploy Ubuntu 22.04 LTS VM `web-nginx` in `web-subnet`, inside `vnet-demo-rg`, with a public IP and inbound SSH (22) and HTTP (80). Use SSH public key or password authentication.

## Evidence

#### Screenshot 4 — VM Overview showing `web-nginx`, its running status, and public IP

Add your screenshot here.

---

#### Screenshot 5 — VM Networking configuration showing `eb-demo-vnet`, `web-subnet`, and inbound rules allowing SSH 22 and HTTP 80

Add your screenshot here.

---

# Task 4 — Install and Configure NGINX

## Goal

Install, enable, and start NGINX on `web-nginx`, then verify the default page through the VM’s public IP.

## Evidence

#### Screenshot 6 — Terminal showing `sudo systemctl status nginx --no-pager` with NGINX active and running

Add your screenshot here.

---

#### Screenshot 7 — Browser showing the NGINX welcome page through the VM Public IP, with the address bar visible

Add your screenshot here.

---

# Task 5 — Create a Public Load Balancer

## Goal

Create Standard Public Load Balancer `web-public-elb` in `vnet-demo-rg`, with frontend public IP `web-elb-ip` and NIC-based backend pool `web-backend-pool` containing `web-nginx`. Configure `web-health-probe` using TCP port 80 with a five-second interval, and associate it with `web-http-rule` using TCP ports 80 → 80.

## Evidence

#### Screenshot 8 — Load Balancer frontend configuration showing its public IP

Add your screenshot here.

---

#### Screenshot 9 — `web-http-rule` configuration showing the frontend, `web-backend-pool`, TCP ports 80 → 80, and `web-health-probe`

Add your screenshot here.

---

# Task 6 — Test the Architecture

## Goal

Confirm that the NGINX default page is accessible through the Load Balancer’s public IP.

## Evidence

#### Screenshot 10 — Browser showing the NGINX welcome page through the Load Balancer Public IP, with the address bar visible

Add your screenshot here.

---

# Task 7 — Clean Up Resources

## Goal

Save Screenshots 1–10, then delete Resource Group `vnet-demo-rg` to avoid ongoing charges.

## Evidence

#### Screenshot 11 — Evidence confirming deletion of `vnet-demo-rg`, such as an Azure success notification or the Resource Groups list showing no results when filtered by its name

Add your screenshot here.

---

# LinkedIn Post (Required)

## Goal

Publish a LinkedIn post sharing your Azure deployment, including a screenshot of NGINX accessed through the Load Balancer’s public IP and three to five lines on what you built, what you learned, and a challenge you resolved. Clarify that only the web-tier VM was deployed and mention resource cleanup. Include **#DMIByPravinMishra #Azure #DevOps #CloudComputing**.

## Evidence

#### LinkedIn Post URL

Paste your LinkedIn post URL here:

`Add your URL here`

---

#### Screenshot 12 — Published LinkedIn post showing your caption and deployment screenshot

Add your screenshot here.

---
# Submission Instructions

- Add Screenshots **1–12** under the corresponding tasks.
- Include your published **LinkedIn post URL**.
- Capture Screenshots **1–10 before deleting the Resource Group**.
- Capture Screenshot **11 after deletion** and Screenshot **12 after publishing your LinkedIn post**.
- Ensure screenshots are readable and meet the full-name requirement in the assignment guidelines.
- Do not expose passwords, private keys, subscription IDs, or other sensitive Azure account information.

---

# Completion Checklist

- [ ] Task 1: Resource Group created (Screenshot 1)
- [ ] Task 2: VNet and three required subnets created (Screenshots 2–3)
- [ ] Task 3: Web VM deployed with the required networking configuration (Screenshots 4–5)
- [ ] Task 4: NGINX running and verified through the VM public IP (Screenshots 6–7)
- [ ] Task 5: Public Load Balancer configured (Screenshots 8–9)
- [ ] Task 6: NGINX reachable through the Load Balancer public IP (Screenshot 10)
- [ ] Task 7: Resource Group deleted after saving deployment evidence (Screenshot 11)
- [ ] LinkedIn post published with the required hashtags (Screenshot 12)
- [ ] LinkedIn post URL included
- [ ] All required screenshots are readable and meet the full-name requirement
- [ ] No sensitive information exposed
---

## 📌 About DMI & CloudAdvisory

DevOps Micro Internship (DMI) is a project-based DevOps program run by Pravin Mishra (The CloudAdvisory) focused on real-world execution, systems thinking, and career readiness.

It helps learners build strong DevOps foundations with hands-on experience.

---

## 📌 Resources

- 🌐 DMI Official Website: https://dmi.pravinmishra.com?utm_source=github&utm_medium=readme  
- 🎓 University: https://university.pravinmishra.com?utm_source=github&utm_medium=readme  
- 💬 Discord Community: https://discord.pravinmishra.com?utm_source=github&utm_medium=readme  
- 📝 Blog: https://dmi.pravinmishra.com/blog?utm_source=github&utm_medium=readme  
- ▶️ YouTube Playlist: https://www.youtube.com/playlist?list=PLFeSNDtI4Cho  
- 🔗 Pravin Mishra (LinkedIn): https://www.linkedin.com/in/pravin-mishra-aws-trainer/  
- 🏢 CloudAdvisory (LinkedIn): https://www.linkedin.com/company/thecloudadvisory/

---

*This submission is part of DevOps Micro Internship (DMI) — Agentic AI Track.*
