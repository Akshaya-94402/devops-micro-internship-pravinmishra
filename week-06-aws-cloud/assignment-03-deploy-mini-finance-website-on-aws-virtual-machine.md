# Assignment 3 — Deploy Mini Finance Website on AWS Virtual Machine

Part of the DevOps Micro Internship (DMI) with Agentic AI

---

## Purpose

In this assignment, you will deploy the Mini Finance static HTML website on an Ubuntu EC2 instance using Nginx. You will launch the instance, configure network access, connect through SSH, install Nginx and Git, deploy the website files, and verify the website through the EC2 public IP address.

---

# Task 1 — Launch an Ubuntu EC2 Instance

## Goal

Launch an Ubuntu EC2 instance named `Mini-Finance-Web-EC2` in a public subnet with a route to an Internet Gateway. Enable a public IPv4 address and confirm the instance is running with passed status checks.

### Evidence

#### Screenshot 1 — EC2 instance details showing the instance name, Running state, passed status checks, and public IPv4 address

Add your screenshot here.

---

# Task 2 — Configure the Security Group

## Goal

Configure the attached security group to allow SSH on port 22 from your IP address only and HTTP on port 80 from Anywhere-IPv4 (`0.0.0.0/0`).

### Evidence

#### Screenshot 2 — Attached security group’s inbound rules showing SSH on port 22 restricted to your IP address and HTTP on port 80 allowed from 0.0.0.0/0

Add your screenshot here.

---

# Task 3 — Connect to the EC2 Instance Using SSH

## Goal

Connect to your Ubuntu EC2 instance using SSH and confirm that you are logged in as the Ubuntu user.

### Evidence

#### Screenshot 3 — Terminal showing a successful SSH connection to the EC2 instance, with the Ubuntu user prompt visible

Add your screenshot here.

---

# Task 4 — Install Nginx and Git

## Goal

Install Nginx and Git. Start Nginx, enable it to start after reboot, and verify that it responds locally.

### Evidence

#### Screenshot 4 — Terminal showing Nginx is active and enabled, the installed Nginx and Git versions, and a successful local HTTP response

Add your screenshot here.

---

# Task 5 — Clone the Mini Finance Website

## Goal

Clone `https://github.com/pravinmishraaws/mini_finance.git` into your home directory and inspect the website files inside `~/mini_finance`.

### Evidence

#### Screenshot 5 — Terminal showing the successful repository clone and the website files listed inside ~/mini_finance

Add your screenshot here.

---

# Task 6 — Copy the Website Files to the Nginx Web Root

## Goal

Replace the default content in `/var/www/html/` with the Mini Finance website files. Set the required ownership and permissions, and verify that the deployed files are present.

### Evidence

#### Screenshot 6 — Terminal showing the output of `ls -la /var/www/html/`, with the deployed website files, ownership, and permissions visible

Add your screenshot here.

---

# Task 7 — Verify Nginx and the Hosted Website

## Goal

Verify the Nginx configuration, restart the service, and test the website locally. Open the EC2 public IP URL in your browser and confirm that Mini Finance loads instead of the default Nginx page.

### Evidence

#### Screenshot 7 — Browser showing the Mini Finance website loaded successfully, with the EC2 public IP URL visible in the address bar

Add your screenshot here.

---

#### Public IP URL

Paste your complete website URL using the format `http://<EC2_PUBLIC_IP>`:

`Add your URL here`

---

# LinkedIn Post (Required)

## Goal

Publish a LinkedIn post sharing your experience deploying the Mini Finance website on an Ubuntu EC2 instance using Nginx.

Include:
- A screenshot of the live Mini Finance website
- Your website URL: `http://<EC2_PUBLIC_IP>`
- A caption in your own words explaining what you deployed, what you learned about EC2, security groups, SSH, and Nginx, and any challenge you resolved

Include these hashtags:

#DMIByPravinMishra #AWS #DevOps #CloudComputing

Add the credit note for your track, replace `YOUR-GITHUB-USERNAME` with your GitHub username, and include the tags specified in the assignment guidelines.

### Evidence

#### LinkedIn Post URL

Paste your LinkedIn post URL here:

`Add your URL here`

---

#### Screenshot 8 — Published LinkedIn post showing your caption, website URL, and live Mini Finance website screenshot

Add your screenshot here.

---

# Submission Instructions

- Add Screenshots 1–7 under their corresponding task headings
- Include the complete EC2 Public IP URL
- Include your LinkedIn Post URL and LinkedIn Screenshot 1
- Ensure screenshots are readable
- Do not expose private keys, passwords, credentials, account IDs, or other sensitive information
- Commit and push the completed submission file to your forked DMI GitHub repository

---

# Completion Checklist

- [ ] Task 1: Ubuntu EC2 instance launched in a public subnet with a public IPv4 address and passed status checks (Screenshot 1)
- [ ] Task 2: SSH allowed from my IP only and HTTP allowed publicly (Screenshot 2)
- [ ] Task 3: Connected to the Ubuntu instance through SSH (Screenshot 3)
- [ ] Task 4: Nginx and Git installed, Nginx active and enabled, and local HTTP response verified (Screenshot 4)
- [ ] Task 5: Mini Finance repository cloned and website files inspected (Screenshot 5)
- [ ] Task 6: Website files copied to `/var/www/html/` with ownership and permissions configured (Screenshot 6)
- [ ] Task 7: Nginx configuration checked and live Mini Finance website verified (Screenshot 7)
- [ ] Complete EC2 Public IP URL included
- [ ] LinkedIn post published with my website screenshot, website URL, and caption written in my own words
- [ ] Required hashtags, track credit note, and tags included
- [ ] LinkedIn Post URL and LinkedIn Screenshot 1 included
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
