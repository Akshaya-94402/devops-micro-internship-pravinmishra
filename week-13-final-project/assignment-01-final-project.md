# DMI with Agentic AI — Cohort 3

# Final Project Submission

Part of the DevOps Micro Internship (DMI) with Agentic AI

**Group Project · Individual Cloud Deployment · Claude Code · Portfolio Evidence**

**Submission deadline:** [To be added by the DMI team]  

**Submission link:** [To be added by the DMI team]

## Student Details

| Field | Your response |
| --- | --- |
| Full name | Add your full name |
| Cohort 3 group | Add your group / squad |
| Final project team name | Add your team name |
| GitHub username | Add your username |
| LinkedIn profile URL | Add your profile URL |
| Group platform repository URL | Add your team’s shared repository URL |
| Individual platform repository URL | Add your individual repository URL |

## Purpose

Build and deploy a platform for the existing Spring Petclinic Microservices application on your selected cloud platform, both as a group and individually. Use **Claude Code** to support platform engineering, review, and troubleshooting, while keeping infrastructure-changing decisions under human control.

## How to Complete This Document

Complete **both Part A and Part B**. Submit **one completed document per student**. Shared team evidence may appear in each member’s submission, but contributions, personal deployment evidence, and reflections must describe your own work.

| Part | Required outcome |
| --- | --- |
| **Part A — Group Project and Presentation** | Work with your team to build a platform for deploying Spring Petclinic to your selected cloud platform, use Claude Code during the platform work, present the solution, and document your contribution. |
| **Part B — Individual Project Deployment** | Personally build and deploy your own platform on your selected cloud platform using Claude Code, verify the application, and document your work. |


**Cloud deployment on AWS or Azure and Claude Code use are mandatory in both parts.** A local-only Docker Compose deployment does not satisfy either part. Local runs may be included as preparation evidence. The group deployment does not replace your individual deployment.


### Cloud and Architecture Choices

Choose **AWS or Azure** for each project and record your choice in A1 and B1. You do not need to deploy to both cloud providers or submit separate dev and prod evidence. Both projects must run on Kubernetes and use Claude Code.

You may adapt the networking, services, resource sizes, deployment tools, and monitoring design to suit your project. NAT gateways and higher-cost resources are allowed. Record significant decisions and their trade-offs in the architecture decision section for each project. No additional screenshots are required for those decisions.


### Repository Responsibilities

| Repository | Purpose | Student responsibility |
| --- | --- | --- |
| [Spring Petclinic Microservices](https://github.com/spring-petclinic/spring-petclinic-microservices) | Existing application source code | Use the supplied application without modifying its application code. |
| Team platform repository | Team infrastructure, deployment automation, platform configuration, documentation, and Claude Code setup | One team member forks the [platform starter repository](https://github.com/pravinmishraaws/petclinic-platform) and adds all team members as collaborators. Use this shared repository, work on separate branches, and review changes through pull requests before merging into `main`. |
| Individual platform repository | Individual infrastructure, deployment automation, platform configuration, documentation, and Claude Code setup | Keep your individual implementation and deployment in a separate repository. |

Platform starter repository: [Petclinic Platform](https://github.com/pravinmishraaws/petclinic-platform). Adapt its cloud-specific configuration for Azure if you choose Azure.

Use the shared team repository for group work and a separate repository for individual work.

Keep platform code and configuration in your platform repository. Use the project guidelines as your starting point and document architecture changes in the decision section below.


### Evidence Instructions

1. Replace every response placeholder with your own answer or link.

2. Include the required repository URLs, presentation links, and evidence.

3. Record the cloud region and deployment date for both projects. Clearly distinguish group evidence from individual evidence.

4. Remove credentials, tokens, private keys, and sensitive values from screenshots and logs. Do not commit secrets or Terraform state files.

5. Capture deployment evidence before cleanup. If the application is unavailable after cleanup, include dated screenshots and verification output.

6. Check that mentors can access your repositories, presentation, recording, screenshots, and published posts.


### Mandatory Agentic AI Evidence — Both Parts

Use Claude Code throughout your platform engineering workflow to support planning, infrastructure development, deployment, review, and troubleshooting. Include screenshots and brief explanations showing how you used Claude Code, reviewed its recommendations, and validated the results.

For **both the group and individual projects**, include focused evidence showing:

- A platform task you completed using Claude Code.

- How Claude Code assisted with implementation, review, or troubleshooting.

- How you reviewed its recommendations and verified the results.

Include relevant screenshots and brief explanations. Review and approve infrastructure changes before applying them.

---

# Part A — Group Project and Presentation

## Task A1 — Team and Presentation Details

### Goal

Record your team, cloud deployment, and presentation details.

### Evidence

| Field | Your response |
| --- | --- |
| Team name | Add your team name |
| Team platform repository URL | Add the repository URL |
| Presentation date | DD Month YYYY |
| Cloud platform | AWS or Azure |
| Cloud region | Add the region |
| Cloud services used | List the services actually used |
| Deployment date | DD Month YYYY |

### Team Members

| Full name | Role / responsibilities | GitHub username | LinkedIn profile URL |
| --- | --- | --- | --- |
| Add name | Add responsibilities | Add username | Add URL |
| Add name | Add responsibilities | Add username | Add URL |
| Add name | Add responsibilities | Add username | Add URL |

Add rows as needed.

---

## Task A2 — Your Individual Contribution

### Goal

Describe your role, the work you personally completed, and what you learned from the group project.

### Your Role and Responsibilities

State your role and list the tasks you personally completed.

**Example:** “I worked on infrastructure provisioning. I configured the Terraform networking modules and verified that the required cloud resources were created successfully.”

Write your response here.

### Evidence

#### Screenshot A2-1 — Your Contribution

Add a screenshot showing one task you personally worked on. This could show your Terraform configuration, deployment pipeline, Kubernetes configuration, monitoring dashboard, or troubleshooting result.

Briefly explain **what the screenshot shows, what you did, and how you confirmed it worked**.

Add your screenshot and explanation here.

### Technical Challenge

Describe one problem you personally helped solve. Explain what went wrong, what you did to resolve it, and how you confirmed the fix.

Write your response here.

### Teamwork Reflection

What did you learn from working with your team?

Write your answer here.

---

## Task A3 — Group Platform and Cloud Deployment Evidence

### Goal

Show your team’s platform architecture and verify that Spring Petclinic runs successfully on your selected cloud platform.

### Architecture Diagram

Add your team’s completed architecture diagram showing the cloud resources, application traffic flow, deployment tools, and monitoring components.

Add your diagram here.

### Architecture Decisions and Changes

Record significant architecture decisions, including changes from the proposed design. Copy the table for each decision you want to explain.

| Field | Your response |
| --- | --- |
| Decision name | Give the decision a short title |
| Decision status | Proposed, Accepted, Superseded, or Rejected |
| Context | Explain the requirement, problem, or constraint |
| Decision | Describe your choice and why you made it |
| Consequences | Explain the benefits and trade-offs, including cost, security, reliability, or operational effort where relevant |

If you followed the proposed architecture without changes, write: **“No architecture changes were made.”**

### Deployment Overview

Briefly explain how your team created the cloud infrastructure and deployed Spring Petclinic. Name the tools used and describe the main deployment steps.

Write your response here.

### Evidence

#### Screenshot A3-1 — Cloud Infrastructure

Add a screenshot showing your team’s deployed cloud resources and the cloud region. Use additional screenshots if the resources cannot be shown clearly in one image.

Add your screenshots here.

---

#### Screenshots A3-2 — Build and Deployment

Add a screenshot of your successful image build-and-push workflow and a screenshot showing the application deployment succeeded. For the reference workflow, show GitHub Actions and ArgoCD applications marked `Synced` and `Healthy`. If you chose different tools, show a successful build and deployment using your chosen tools and explain the choice in your architecture decisions.

Add your screenshot here.

---

#### Screenshot A3-3 — Application Running on your selected cloud platform

Open the deployed Spring Petclinic application and capture its homepage with the application URL visible in the browser.

Add your screenshot here.

**Application URL:** Add your application URL here.

---

#### Screenshot A3-4 — Kubernetes Pod Status

Run `kubectl get pods -n <application-namespace>` and add a screenshot showing all application pods in the Running state, with all containers ready in the READY column.

Add your screenshot here.

---

#### Screenshots A3-5 — Application Functionality

Add screenshots showing:

- The owners list.

Add your screenshot here.

- An owner’s pet details and visit history.

Add your screenshot here.

- A newly added visit appearing in the application.

Add your screenshot here.

- The veterinarians list.

Add your screenshot here.

---

#### Screenshot A3-6 — Monitoring Dashboard

Add a screenshot of your monitoring dashboard displaying metrics from the cloud deployment. Briefly explain what one of the displayed metrics tells you.

Add your screenshot here.

Add your explanation here.

---

#### Screenshot A3-7 — Request Trace

Generate activity in the application, then find a corresponding request trace in Zipkin or your chosen tracing tool. Add a screenshot showing the services involved in that request.

Add your screenshot here.

Add your explanation here.

---

### Security and Configuration

Briefly answer each question:

1. How did your team control access to the application and internal services?

Write your answer here.

2. How did your team store and supply secrets?

Write your answer here.

3. How did your team provide configuration to the application?

Write your answer here.

---

## Task A4 — Group Agentic AI Evidence — Required

### Goal

Demonstrate how your team used Claude Code for the group project and explain your own involvement.

### Task You Worked On

Choose **one task** you personally completed or reviewed using Claude Code—for example, configuring Terraform, reviewing Kubernetes manifests, or troubleshooting a deployment.

**What was the task, and what did you personally do?**

Write your response here.

### Evidence

#### Screenshot A4-1 — Working with Claude Code

Add a screenshot showing your request to Claude Code and its response or actions for the chosen task. Use additional screenshots if needed.

Add your screenshot here.

**Briefly explain how Claude Code helped you complete the task.**

Write your response here.

---

#### Screenshot A4-2 — Review and Verification

Add a screenshot showing how you checked the result—for example, successful Terraform validation, a successful pipeline run, or Kubernetes pods running with all containers ready.

Add your screenshot here.

**What did you check before accepting Claude Code’s work? Mention any recommendation you corrected or rejected, if applicable.**

Write your response here.

**How did you confirm that the result worked?**

Write your response here.

### Claude Code Features Used

Which of the following supported your chosen task: `CLAUDE.md`, skills, subagents, MCP connections, or hooks?

Name the features used and briefly explain how they helped. You do not need to attach their configuration files.

Write your response here.

**Complete this section based on your own participation in the group project.**

---

## Task A5 — Presentation and Demo

### Goal

Present your group project, demonstrate the working cloud deployment, and explain each member’s contribution.

### Presentation Requirements

Cover the architecture, cloud deployment, automation, Claude Code use, application verification, observability, and challenges.

**Each team member must present their own contribution during the live demo**, explaining what they worked on and demonstrating or showing the results.

### Evidence

| Item | Link |
| --- | --- |
| Presentation slides | Add URL |
| Group presentation recording | Add the YouTube link starting at your group’s presentation |
| Your individual presentation section | Add the YouTube link starting when you present your contribution |

Use YouTube’s **Share → Start at** option to copy each timestamped link.

---

## Task A6 — LinkedIn Post — Group Project

### Goal

Publish a LinkedIn post sharing your group’s cloud deployment, your personal contribution, and your experience using Claude Code.

### Post Requirements

Write the post in your own words. Suggested length: **150–300 words**.

Include:

- What your team built and deployed to AWS or Azure using Kubernetes.
- Your personal contribution and one technical lesson.
- How your team used Claude Code and verified its work.
- A screenshot of the working application.
- Your platform architecture diagram.
- A screenshot of you presenting your contribution during the group presentation.
- Your team platform repository link.
- Tags for your teammates, Pravin Mishra, and your co-mentors.

Include these hashtags and add **#AWS** or **#Azure** for your selected cloud platform:

**#DMIByPravinMishra #DevOps #AgenticAI #CloudComputing**

### Required Credit Note

Add the following at the end of your post. Replace `YOUR-GITHUB-USERNAME` with your GitHub username and tag Pravin Mishra using LinkedIn’s tagging feature.

**P.S. This post is part of the DevOps Micro Internship (DMI) with Agentic AI — Cohort 3 — by [Pravin Mishra](https://www.linkedin.com/in/pravin-mishra-aws-trainer/). My graded progress is public: https://dmi.pravinmishra.com/s/YOUR-GITHUB-USERNAME.html · Start your DevOps journey: https://dmi.pravinmishra.com/?utm_source=student&utm_medium=ps-linkedin&utm_campaign=cohort3**

**Interested in joining DMI Cohort 4?** Join the waiting list to receive program details and next steps: https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform

### Evidence

#### LinkedIn Post URL

Paste your published LinkedIn post URL here:

`Add your URL here`

---

#### Screenshot A6-1 — Published LinkedIn Post

Add a screenshot showing your published caption, project image, and required credit note. Use additional screenshots if the full post does not fit in one image.

Add your screenshot here.

---

## Task A7 — Blog — Group Project

### Goal

Publish a blog explaining your group project, your personal contribution, and what you learned.

### Blog Requirements

Write the blog in your own words. Suggested length: **500–800 words**.

Include:

- An overview of the platform your team built and deployed to your selected cloud platform using Kubernetes.
- Your architecture diagram and an explanation of its main components.
- Your personal role and the tasks you completed.
- How your team used Claude Code and verified its work.
- How you tested the application and checked its monitoring data.
- One challenge you helped resolve and what you learned.
- Relevant screenshots and your team platform repository link.

Suggested platforms: **Hashnode, Substack, a public Notion page, or HackerNoon**. Choose a platform you do not already publish on regularly.

### Required Credit Note

Add the following at the end of your blog. Replace `YOUR-GITHUB-USERNAME` with your GitHub username.

**P.S. This post is part of the DevOps Micro Internship (DMI) with Agentic AI — Cohort 3 — by [Pravin Mishra](https://www.linkedin.com/in/pravin-mishra-aws-trainer/). My graded progress is public: https://dmi.pravinmishra.com/s/YOUR-GITHUB-USERNAME.html · Start your DevOps journey: https://dmi.pravinmishra.com/?utm_source=student&utm_medium=ps-blog&utm_campaign=cohort3**

**Interested in joining DMI Cohort 4?** Join the waiting list to receive program details and next steps: [https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform](https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform)

### Evidence

| Field | Your response |
| --- | --- |
| Blog platform | Add your platform |
| Blog title | Add your blog title |
| Published blog URL | Add your published blog URL |

Ensure that the published blog and its images can be viewed by the submission reviewer.

---

# Part B — Individual Cloud Deployment

Complete this part personally. Include evidence of your own platform work, Claude Code workflow, cloud deployment, and verification.

## Task B1 — Deployment Details

### Goal

Record your individual platform repository and cloud deployment details.

### Evidence

| Field | Your response |
| --- | --- |
| Individual platform repository URL | Add your repository URL |
| Cloud platform | AWS or Azure |
| Cloud region | Add the region |
| Cloud services used | List the services you used |
| Deployment date | DD Month YYYY |
| Application URL | Add your application URL |

---

## Task B2 — Platform Repository and Architecture

### Goal

Show your individual platform architecture and explain how your repository is organized.

### Evidence

### Architecture Diagram

Add your architecture diagram showing the cloud resources, Kubernetes cluster, application traffic flow, deployment tools, and monitoring components.

Add your diagram here.

### Architecture Decisions and Changes

Record significant architecture decisions, including changes from the proposed design. Copy the table for each decision you want to explain.

| Field | Your response |
| --- | --- |
| Decision name | Give the decision a short title |
| Decision status | Proposed, Accepted, Superseded, or Rejected |
| Context | Explain the requirement, problem, or constraint |
| Decision | Describe your choice and why you made it |
| Consequences | Explain the benefits and trade-offs, including cost, security, reliability, or operational effort where relevant |

If you followed the proposed architecture without changes, write: **“No architecture changes were made.”**

---

#### Screenshot B2-1 — Platform Repository Structure

Add a screenshot of your platform repository’s folder structure in VS Code or GitHub.

Below the screenshot, identify the folders containing:

- Terraform infrastructure code.

- Kubernetes deployment files, Helm charts, and Helm values where used.

- CI/CD and ArgoCD configuration, or the deployment tools you selected.

- Claude Code configuration.

- Project documentation.

Add your screenshot and brief explanation here.

---

## Task B3 — Individual Agentic AI Evidence — Required

### Goal

Demonstrate how you used Claude Code during your individual project and verified its work.

### Task You Worked On

Choose **one task** you completed using Claude Code—for example, configuring Terraform, reviewing Kubernetes manifests, or troubleshooting a deployment.

**What was the task, and how did Claude Code help?**

Write your response here.

### Evidence

#### Screenshot B3-1 — Working with Claude Code

Add a screenshot showing your request to Claude Code and its response or actions for the chosen task. Use additional screenshots if needed.

Add your screenshot here.

---

#### Screenshot B3-2 — Verification Result

Add a screenshot showing how you verified the result—for example, successful Terraform validation, a successful pipeline run, or Kubernetes pods showing `Running` with all containers ready.

Add your screenshot here.

**What did you check before accepting Claude Code’s work? Mention any recommendation you corrected or rejected, if applicable.**

Write your response here.

**How did you confirm that the result worked?**

Write your response here.

### Claude Code Features Used

Which features supported your chosen task: `CLAUDE.md`, skills, subagents, MCP connections, or hooks?

Name the features used and briefly explain how they helped. You do not need to attach their configuration files.

Write your response here.

**Use evidence from your individual project for this section.**

---

## Task B4 — Cloud Provisioning and Deployment

### Goal

Create the required cloud infrastructure and deploy Spring Petclinic to Kubernetes using your platform.

### Step 1 — Prepare the Environment

#### Prerequisites and Configuration

List the tools and configuration needed to run your deployment. Include the relevant configuration file names and required variable names. Do not include secret values.

Write your response here.

#### Commands Used

Paste the commands you used to obtain your platform repository and prepare the application source or container images. If your pipeline performs these steps, provide the pipeline file link instead.

```text
Paste your commands or pipeline file link here.
```

### Step 2 — Provision your selected cloud platform Resources

### Infrastructure Provisioning

Briefly explain how you created the cloud infrastructure. Include the commands you ran or the provisioning pipeline link.

Write your response here.

#### Screenshot B4-1 — Successful Infrastructure Provisioning

Add a screenshot showing successful infrastructure provisioning. For Terraform, show the completed `terraform apply` output. If provisioning runs through a pipeline, show the successful run.

Include the reviewed plan summary if your workflow uses a plan and approval step.

Add your screenshot here.

---

#### Screenshot B4-2 — Cloud Resources

Add screenshots showing the cloud resources created for your individual project, with the cloud region visible. Use additional screenshots where needed.

Add your screenshots here.

### Step 3 — Deploy the Application

### Deployment Method

Briefly explain how you deployed Spring Petclinic to Kubernetes. Include the commands you ran or the deployment pipeline link.

Write your response here.

#### Screenshots B4-3 — Build and Application Deployment

Add a screenshot of your successful image build-and-push workflow and a screenshot showing the application deployment succeeded. For the reference workflow, show GitHub Actions and ArgoCD applications marked `Synced` and `Healthy`. If you chose different tools, show equivalent results and explain the choice in your architecture decisions.

Add your screenshot here.

---

#### Screenshot B4-4 — Kubernetes Pod Status

Run:

```bash
kubectl get pods -n <application-namespace>
```

Replace `<application-namespace>` with your application’s namespace.

Add a screenshot showing the application pods in the `Running` state, with all containers ready in the `READY` column. Explain any pods that are not running or ready.

Add your screenshot here.

### Startup Dependencies

Briefly explain:

1. How the application services receive their configuration.
Write your answer here.

2. How services discover and connect to one another.
Write your answer here.

3. How your deployment checks that services are ready to receive traffic.
Write your answer here.

---

## Task B5 — Application Verification in the Cloud

### Goal

Verify that Spring Petclinic works correctly through your individual cloud deployment.

### Application URL

**Application URL:** Add your deployed application URL here.

Complete the following checks using this deployment.

### Evidence

#### Screenshot B5-1 — Application Homepage

Open your application URL and add a screenshot showing the Spring Petclinic homepage, with the URL visible in the browser.

Add your screenshot here.

---

#### Screenshot B5-2 — Owners List

Navigate to **Find Owners** and search without entering a name. Add a screenshot showing the returned owners list.

Add your screenshot here.

---

#### Screenshot B5-3 — Pet Details and Visit History

Open an owner’s details. Add a screenshot showing their pets and visit history.

Add your screenshot here.

---

#### Screenshot B5-4 — Add a Visit

Add a visit for a pet using demonstration data. Submit it, then capture a screenshot showing the new visit in the pet’s visit history.

Add your screenshot here.

---

#### Screenshot B5-5 — Veterinarians List

Open the **Veterinarians** page. Add a screenshot showing the veterinarians and their specialties.

Add your screenshot here.

### Functional Test Summary

Briefly state whether all five checks passed. If any check failed, describe the issue and its current status.

Write your response here.

---

## Task B6 — Observability Verification

### Goal

Verify service registration, application health, metrics, dashboards, and request traces for your individual cloud deployment.

### Evidence

Use the tools listed below, or the equivalent tools selected for your architecture. If you used an alternative, name it and provide evidence of the same check. Explain the change in your architecture decisions.

#### Screenshot B6-1 — Eureka Service Registration

Open the Eureka dashboard. Take a screenshot showing the registered application services.

Add your screenshot here.

**List the registered services. If an expected service is missing, explain why.**

Write your answer here.

---

#### Screenshot B6-2 — Application Health

Open Spring Boot Admin. Take a screenshot showing the application services and their health status.

Add your screenshot here.

**Are the services healthy? Explain any service reporting a problem.**

Write your answer here.

---

#### Screenshot B6-3 — Prometheus Metrics

Generate application traffic by browsing owners, pet details, or veterinarians. Open Prometheus and run a query for an application request metric, such as `http_server_requests_seconds_count`, if available.

Take a screenshot showing the query and its result.

Add your screenshot here.

**What does this metric measure, and what does your result show?**

Write your answer here.

---

#### Screenshot B6-4 — Grafana Dashboard

Open a Grafana dashboard displaying metrics from your cloud deployment. Take a screenshot showing panels with data.

Add your screenshot here.

**Choose one panel and briefly explain what it shows about your application.**

Write your answer here.

---

#### Screenshot B6-5 — Zipkin Request Trace

Perform an action in Spring Petclinic, such as searching for owners. Open Zipkin, find a trace from that activity, and open its details.

Take a screenshot showing the trace and the services involved.

Add your screenshot here.

**Which services appear in the trace, and what does it show about the request’s flow?**

Write your answer here.

---

## Task B7 — Troubleshooting and Validation

### Goal

Describe one issue you investigated during your individual project, how you resolved it, and how you verified the result.

### Issue and Resolution

Briefly answer the following:

1. **What went wrong?** Describe the problem and any error message you received.

   Write your answer here.

2. **How did you investigate it?** Explain which logs, Kubernetes events, or command outputs you checked and what you found.

   Write your answer here.

3. **What caused the problem, and how did you fix it?**

   Write your answer here.

4. **How did Claude Code help?** Explain its role and how you reviewed its recommendations. If you solved this issue without Claude Code, state that.

   Write your answer here.

### Evidence

#### Screenshot B7-1 — Problem or Investigation

Add a screenshot showing the error or the logs, events, or command output you used to investigate it.

Add your screenshot here.

---

#### Screenshot B7-2 — Verification After the Fix

Add a screenshot showing that the issue was resolved—for example, a successful pipeline run, application functionality restored, or Kubernetes pods running with all containers ready.

Add your screenshot here.

**Briefly explain how this result confirms the fix worked.**

Write your answer here.

---

If you did not encounter an issue, describe one validation check you performed, what you investigated, and what the result confirmed. Include screenshots of the check and its result.

---

## Task B8 — Cleanup and Cost Control

### Goal

Remove the cloud resources created for your individual project and check for any remaining resources that could incur charges.

### Cleanup

Capture all required deployment screenshots before removing resources.

**What commands or automation did you use to remove your resources?**

Paste your cleanup commands or automation run link here.

### Evidence

#### Screenshot B8-1 — Cleanup Result

Add a screenshot showing successful cleanup—for example, completed `terraform destroy` output or a successful cleanup pipeline run.

Add your screenshot here.

---

#### Screenshot B8-2 — Remaining Resources

Check the AWS or Azure portal for any remaining project resources, including:

- Kubernetes clusters and worker nodes, such as EKS or AKS.

- Load balancers.

- Disks, volumes, and snapshots.

- NAT gateways, if created, and allocated public IP addresses.

- Databases, container registries, and any other resources created for your project.

Add screenshots showing the results of your checks.

Add your screenshots here.

**Did any project resources remain?** If yes, list them, explain why they remain, whether they could incur charges, and when you will remove them. Otherwise, state that no project resources remain.

Write your answer here.

---

## Task B9 — Personal Reflection

### Goal

Reflect on your individual project, technical decisions, and experience using Claude Code.

### Reflection Questions

Answer each question briefly in your own words.

#### 1. What was the most challenging part of deploying your platform to your selected cloud platform, and how did you handle it?

Write your answer here.

#### 2. What belongs in your platform repository, and how is it different from the application repository?

Write your answer here.

#### 3. How did Claude Code help you, and which decisions did you make yourself?

Write your answer here.

#### 4. How did you verify that the application worked beyond checking that the Kubernetes pods were running?

Write your answer here.

#### 5. How did you manage secrets, control network access, and provide configuration to the application?

Write your answer here.

#### 6. What would you improve before using this platform for a real production workload, and why?

Write your answer here.

#### 7. What did completing the individual project teach you that the group project did not?

Write your answer here.

---

## Task B10 — LinkedIn Post — Individual Cloud Deployment

### Goal

Publish a separate LinkedIn post sharing your individual cloud deployment, what you learned, and how you used Claude Code.

### Post Requirements

Write the post in your own words. Suggested length: **150–300 words**.

Include:

- What you personally built and deployed to AWS or Azure using Kubernetes.
- The main tools used and any architecture decision you want to highlight.
- How you used Claude Code and verified its work.
- A challenge you resolved or a technical lesson you learned.
- A screenshot of your working application.
- Your platform architecture diagram.
- Your individual platform repository link and application URL.
- Tags for Pravin Mishra and your co-mentors.

If you removed the cloud resources after verification, mention that the deployment was cleaned up.

Include these hashtags and add **#AWS** or **#Azure** for your selected cloud platform:

**#DMIByPravinMishra #DevOps #AgenticAI**

### Required Credit Note

Add the following at the end of your post. Replace `YOUR-GITHUB-USERNAME` with your GitHub username and tag Pravin Mishra using LinkedIn’s tagging feature.

**P.S. This post is part of the DevOps Micro Internship (DMI) with Agentic AI — Cohort 3 — by [Pravin Mishra](https://www.linkedin.com/in/pravin-mishra-aws-trainer/). My graded progress is public: https://dmi.pravinmishra.com/s/YOUR-GITHUB-USERNAME.html · Start your DevOps journey: https://dmi.pravinmishra.com/?utm_source=student&utm_medium=ps-linkedin&utm_campaign=cohort3**

**Interested in joining DMI Cohort 4?** Join the waiting list to receive program details and next steps: [https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform](https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform)

### Evidence

#### LinkedIn Post URL

Paste your published LinkedIn post URL here:

`Add your URL here`

---

#### Screenshot B10-1 — Published LinkedIn Post

Add a screenshot showing your published caption, project image, and required credit note. Use additional screenshots if the full post does not fit in one image.

Add your screenshot here.

---

## Task B11 — Blog — Individual Cloud Deployment

### Goal

Publish a technical walkthrough explaining your individual cloud deployment, architecture decisions, and experience using Claude Code.

### Blog Requirements

Write the blog in your own words. Suggested length: **700–1,200 words**.

Include:

- An overview of Spring Petclinic and the purpose of your platform repository.
- Your AWS or Azure architecture diagram and the prerequisites for deployment.
- Any significant architecture changes, why you made them, and their trade-offs.
- Infrastructure provisioning and Kubernetes deployment steps, with relevant commands and configuration examples.
- How you used Claude Code, reviewed its recommendations, and verified the results.
- Screenshots of the working application, functionality checks, and monitoring results.
- A challenge you resolved and what you learned.
- How you cleaned up cloud resources and checked for remaining costs.
- Your individual platform repository link and application URL, if publicly accessible.

### Required Credit Note

Add the following at the end of your blog. Replace `YOUR-GITHUB-USERNAME` with your GitHub username.

**P.S. This post is part of the DevOps Micro Internship (DMI) with Agentic AI — Cohort 3 — by [Pravin Mishra](https://www.linkedin.com/in/pravin-mishra-aws-trainer/). My graded progress is public: https://dmi.pravinmishra.com/s/YOUR-GITHUB-USERNAME.html · Start your DevOps journey: https://dmi.pravinmishra.com/?utm_source=student&utm_medium=ps-blog&utm_campaign=cohort3**

**Interested in joining DMI Cohort 4?** Join the waiting list to receive program details and next steps: [https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform](https://docs.google.com/forms/d/e/1FAIpQLSdJTrzJi33PvpccoAiPOaN2RuYpPEk_ltzRQsEqM6YbkYEBCg/viewform)

### Evidence

**Blog platform:** Add your platform here.

**Blog title:** Add your blog title here.

#### Published Blog URL

Paste your published blog URL here:

`Add your URL here`

Ensure that the published blog and its images can be viewed by the submission reviewer.

---

## Submission Instructions

- Complete Tasks A1–A7 and B1–B11.

- Submit one completed Markdown document per student through the assignment submission GitHub repository, following the cohort folder and filename instructions.

- Include all requested screenshots, answers, architecture diagrams, repository links, presentation slides, and presentation recording.

- Include **two LinkedIn post URLs and two blog URLs**—one of each for the group project and individual project.

- Add the required credit note. Replace `YOUR-GITHUB-USERNAME` with your GitHub username.

- Store screenshots in an accessible evidence folder and use working image links.

- Clearly distinguish group-project evidence from individual-project evidence.

- Review all screenshots, logs, and files for credentials and sensitive information before submitting.

## Completion Checklist

### Part A — Group Project

- [ ] Team details, team members, cloud region, and deployment date are recorded.

- [ ] The team platform repository, architecture diagram, and architecture decisions or no-change statement are included.

- [ ] My role, completed tasks, contribution screenshot, technical challenge, and teamwork reflection are complete.

- [ ] Group cloud deployment, Kubernetes pod status, and application functionality screenshots are included.

- [ ] Group monitoring and request-tracing evidence are included.

- [ ] Claude Code evidence shows my participation, review, and verification.

- [ ] Presentation slides and recording are linked and accessible.

- [ ] My group-project LinkedIn post is published, with its URL and screenshot included.

- [ ] My group-project blog is published and linked.

### Part B — Individual Project

- [ ] My individual platform repository, cloud region, deployment date, cloud services, and application URL are recorded.

- [ ] My architecture diagram, repository structure screenshot, and architecture decisions or no-change statement are included.

- [ ] I personally deployed the application to my selected cloud platform, separately from the group deployment.

- [ ] Claude Code evidence shows my own workflow, review, and verification.

- [ ] Cloud provisioning, application deployment, and Kubernetes pod status screenshots are included.

- [ ] Homepage, owners, pet details, visit history, newly added visit, and veterinarians checks are complete.

- [ ] Service discovery, application health, metrics, dashboard, and tracing evidence and explanations are included.

- [ ] Troubleshooting or validation evidence is included.

- [ ] Cleanup evidence and any remaining resources are documented.

- [ ] All personal reflection questions are answered.

- [ ] My individual-project LinkedIn post is published, with its URL and screenshot included.

- [ ] My individual-project blog is published and linked.

### Document Quality

- [ ] Application code was not modified; platform changes are in the platform repositories.

- [ ] All response placeholders have been replaced.

- [ ] Screenshots are readable, labelled, and accessible.

- [ ] Repository links, presentation links, published posts, and images are accessible to reviewers.

- [ ] Both LinkedIn posts and both blogs include the required credit note.

- [ ] My GitHub username is correctly inserted in each graded-progress URL.

- [ ] No credentials, secrets, or sensitive information are exposed.

- [ ] Group evidence and individual evidence are clearly distinguished.

- [ ] I have completed the submission requirements and explained significant architecture decisions or changes.

## Student Declaration

I confirm that this submission accurately represents my group contributions and individual deployment. I have documented my use of Claude Code, reviewed its outputs, and can explain the platform configuration, technical decisions, and verification evidence submitted.

**Full name:** Add your full name  

**Date:** DD Month YYYY

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
