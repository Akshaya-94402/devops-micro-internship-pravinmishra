# Assignment 4 — Deploy EpicBook on Ubuntu VM + MySQL RDS with Secure Cloud Network

Part of the DevOps Micro Internship (DMI) with Agentic AI

---

## Purpose

In this assignment, you will deploy the EpicBook web application in AWS using a secure two-tier architecture: an Ubuntu EC2 instance with Nginx in a public subnet, and a private MySQL RDS database with restricted security-group access. The completed deployment must prove that the frontend, backend, and private database communicate successfully end to end.

---

# Task 1 — Create VPC + Public/Private Subnets + Routing

## Goal

Create the AWS network for the EpicBook deployment with a public subnet for the EC2 instance and private subnets for Amazon RDS MySQL.

### Evidence

#### Screenshot 1 — VPC details showing CIDR 10.0.0.0/16

Add your screenshot here.

---

#### Screenshot 2 — Subnets list showing the public subnet and both private database subnets with their CIDR ranges.

Add your screenshot here.

---

#### Screenshot 3 — Route table showing 0.0.0.0/0 → IGW and association with the public subnet

Add your screenshot here.

---

# Task 2 — Create Security Groups (EC2 + RDS) with Least Privilege

## Goal

Create security groups that allow users to access the EpicBook application while restricting database access to the EC2 instance.

### Evidence

#### Screenshot 4 — EC2 security-group inbound rules showing ports and sources

Add your screenshot here.

---

#### Screenshot 5 — RDS security-group inbound rule showing MySQL 3306 allowed from the EC2 security group

Add your screenshot here.

---

# Task 3 — Launch Ubuntu EC2 in Public Subnet

## Goal

Launch the EC2 instance that will host the EpicBook application and connect to it through SSH.

### Evidence

#### Screenshot 6 — EC2 instance summary showing the public IPv4 address, subnet, and security group

Add your screenshot here.

---

#### Screenshot 7 — Terminal showing a successful SSH login with the `ubuntu@...` prompt

Add your screenshot here.

---

# Task 4 — Install Required Software on EC2

## Goal

Prepare Ubuntu to download and run EpicBook, receive HTTP traffic, and connect to RDS.

### Evidence

#### Screenshot 8 — Output of `node -v` and `npm -v`

Add your screenshot here.

---

#### Screenshot 9 — Output of `systemctl status nginx`

Add your screenshot here.

---

#### Screenshot 10 — Output of `mysql --version`

Add your screenshot here.

---

# Task 5 — Create RDS MySQL in Private Subnet (No Public Access)

## Goal

Launch a private MySQL database accessible only from the application EC2 security group.

### Evidence

#### Screenshot 11 — RDS instance summary showing Publicly accessible: No

Add your screenshot here.

---

#### Screenshot 12 — Connectivity & security section showing the VPC and attached security group

Add your screenshot here.

---

# Task 6 — Initialize Database (SQL Dump Import)

## Goal

Download EpicBook and populate bookstore with the schema, authors, and books required by the application.

### Evidence

#### Screenshot 13 — Terminal showing successful `SHOW TABLES;` output with tables listed

Add your screenshot here.

---

# Task 7 — Deploy EpicBook Backend and Configure Environment Variables

## Goal

Run EpicBook on port 8080 and connect its Sequelize models to bookstore in RDS.

### Evidence

#### Screenshot 14 — Terminal showing the repository cloned and the `ls` output

Add your screenshot here.

---

#### Screenshot 15 — Terminal showing EpicBook running, or ss -tulpn output showing port 8080 listening

Add your screenshot here.

---

#### Screenshot 16 — `curl` output proving the backend responds; a 200, 301, or 404 response is acceptable if the service responds

Add your screenshot here.

---

# Task 8 — Configure Nginx as a Reverse Proxy and Enable Persistence.

## Goal

Expose EpicBook through Nginx on port 80 and keep its Node.js process running after SSH disconnects and server reboots.

### Evidence

#### Screenshot 17 — `nginx -t` success output

Add your screenshot here.

---

#### Screenshot 18 — Nginx configuration snippet showing location / forwarding requests to http://127.0.0.1:8080

Add your screenshot here.

---

# Task 9 — End-to-End Testing (Frontend ↔ Backend ↔ RDS)

## Goal

Verify the public application and its use of the imported RDS data.

### Evidence

#### Screenshot 19 — Browser showing the EpicBook application loaded with the public IP visible

Add your screenshot here.

---

#### Screenshot 20 — Terminal showing a successful HTTP request to EpicBook through the public Nginx endpoint using curl -i http://<EC2_PUBLIC_IP>/

Add your screenshot here.

---

#### Screenshot 21 — Terminal showing the successful database connectivity test using `SELECT 1;` or similar

Add your screenshot here.

---

# LinkedIn Post (Required)

## Goal

Publish a LinkedIn post sharing your experience deploying EpicBook on an Ubuntu EC2 instance with Nginx and a private Amazon RDS MySQL database.

Include:
- A screenshot of the live EpicBook application showing the book listing
- Your application URL: `http://<EC2_PUBLIC_IP>/`
- A caption in your own words explaining what you deployed, how the main components connect, and what you learned about network security, Nginx, and PM2
- One challenge you faced and how you resolved it, if applicable

Include these hashtags:

#DMIByPravinMishra #AWS #DevOps #CloudComputing

Add the credit note for your track, replace `YOUR-GITHUB-USERNAME` with your GitHub username, and include the tags specified in the assignment guidelines.

## Evidence

#### LinkedIn Post URL

Paste your LinkedIn post URL here:

`Add your URL here`

---

#### Screenshot 22 — Published LinkedIn post showing your caption, application URL, and live EpicBook screenshot

Add your screenshot here.

> **Privacy Note:** Do not expose passwords, private keys, `.env` values, database credentials, or sensitive AWS account information.

---

# Submission Instructions

- Add all required screenshots in your submission
- Do not expose PEM contents, passwords, `.env` values, or other secrets

---

# Completion Checklist

- [ ] Task 1: VPC, public/private subnets, IGW, and public routing created (Screenshots 1–3)
- [ ] Task 2: Least-privilege EC2 and RDS security groups created (Screenshots 4–5)
- [ ] Task 3: Ubuntu EC2 launched in the public subnet with SSH verified (Screenshots 6–7)
- [ ] Task 4: Node.js, npm, Nginx, and MySQL client, Git installed (Screenshots 8–10)
- [ ] Task 5: Private MySQL RDS created with no public access (Screenshots 11–12)
- [ ] Task 6: Database initialized from the SQL dump (Screenshot 13)
- [ ] Task 7: Backend deployed and responding on port 8080 (Screenshots 14–16)
- [ ] Task 8: Nginx proxying requests to EpicBook, with PM2 persistence. (Screenshots 17–18)
- [ ] Task 9: Frontend, backend, and RDS verified end to end (Screenshots 19–21)
- [ ] No sensitive data exposed
- [ ] LinedIn post published

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
