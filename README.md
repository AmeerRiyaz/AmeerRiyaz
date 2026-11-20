<div align="center">

<img src="./banner.svg" width="100%" alt="Ameer Riyaz - Senior Project Engineer, DevOps and Platform Engineering" />

<a href="https://github.com/AmeerRiyaz">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=750&height=45&lines=terraform+apply+-auto-approve;kubectl+get+nodes+%28HA+cluster+ready%29;ansible-playbook+site.yml;argocd+app+sync+production;Architecting+apps+for+government+%26+enterprise" alt="Typing SVG" />
</a>

<br/><br/>

![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?logo=terraform&logoColor=white&style=for-the-badge)
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white&style=for-the-badge)
![AWS](https://img.shields.io/badge/-AWS-232F3E?logo=amazonaws&logoColor=white&style=for-the-badge)
![Ansible](https://img.shields.io/badge/-Ansible-EE0000?logo=ansible&logoColor=white&style=for-the-badge)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white&style=for-the-badge)
![Helm](https://img.shields.io/badge/-Helm-0F1689?logo=helm&logoColor=white&style=for-the-badge)

![Profile views](https://komarev.com/ghpvc/?username=AmeerRiyaz&label=Profile+Views&color=7B42BC&style=for-the-badge)
![Followers](https://img.shields.io/github/followers/AmeerRiyaz?label=Followers&style=for-the-badge&color=326CE5&logo=github)
![Location](https://img.shields.io/badge/Hyderabad,_India-7B42BC?logo=googlemaps&logoColor=white&style=for-the-badge)

<br/>

[![About](https://img.shields.io/badge/About-7B42BC?style=flat-square)](#about)
[![Pipeline](https://img.shields.io/badge/Pipeline-326CE5?style=flat-square)](#pipeline)
[![Architecture](https://img.shields.io/badge/HA_Architecture-326CE5?style=flat-square)](#architecture)
[![Toolbox](https://img.shields.io/badge/Toolbox-7B42BC?style=flat-square)](#toolbox)
[![Journey](https://img.shields.io/badge/Journey-326CE5?style=flat-square)](#journey)
[![Certifications](https://img.shields.io/badge/Certifications-7B42BC?style=flat-square)](#certs)
[![Stats](https://img.shields.io/badge/Stats-326CE5?style=flat-square)](#stats)
[![Contact](https://img.shields.io/badge/Contact-7B42BC?style=flat-square)](#contact)

<br/>

[![Download Resume](https://img.shields.io/badge/Download-Resume_PDF-7B42BC?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](./Shaik_Ameer_Riyaz_Resume.pdf)

</div>

---

<a id="about"></a>
## ⚙️ About Me

I design, build and run distributed applications for government and enterprise clients at **C-DAC, Hyderabad**. I own solution architecture and design, build HA and standard Kubernetes clusters on AWS and on-premise, and automate everything with Terraform and Ansible. My domain specialty is **Hyperledger Fabric** and **Besu**.

```hcl
# profile.tf
locals {
  engineer = {
    name         = "Ameer Riyaz"
    role         = "Senior Project Engineer @ C-DAC"
    location     = "Hyderabad, India"
    experience   = "5+ years"
    focus        = ["IaC", "Kubernetes HA", "CI/CD + GitOps", "Event-driven backends"]
    domain       = ["Hyperledger Fabric", "Hyperledger Besu"]
    certified    = ["CKAD", "Fabric Practitioner", "Besu Professional"]
    open_to_chat = true
  }
}
```

---

## 🔄 How I Ship

```mermaid
flowchart LR
    A[Code] --> B[GitLab CI / Jenkins]
    B --> C[Docker Image]
    C --> D[Helm Chart]
    D --> E[Argo CD]
    E --> F[(Kubernetes: HA or standard)]
    G[Terraform] -.provisions.-> H[AWS / On-premise]
    I[Ansible] -.configures.-> H
    H --> F
    F --> J[Prometheus + Grafana]
```

<a id="pipeline"></a>
### ⚡ Live Pipeline

<div align="center">

<img src="./pipeline.svg" width="100%" alt="Animated delivery pipeline from code to Kubernetes" />

</div>

---

<a id="architecture"></a>
## 🏗️ HA Kubernetes Reference Architecture

A reference topology for the highly available clusters I build with Terraform and Ansible.

```mermaid
flowchart TB
    U([Users / Clients]) --> LB{{Load Balancer}}
    LB --> CP1
    LB --> CP2
    LB --> CP3

    subgraph CP[Control Plane - highly available]
        CP1[Control Plane Node 1]
        CP2[Control Plane Node 2]
        CP3[Control Plane Node 3]
        ETCD[(etcd cluster)]
        CP1 --- ETCD
        CP2 --- ETCD
        CP3 --- ETCD
    end

    CP1 --> W1
    CP2 --> W2
    CP3 --> W3

    subgraph WK[Worker Nodes]
        W1[Worker 1]
        W2[Worker 2]
        W3[Worker 3]
    end

    W1 --> ING[Ingress / Services]
    W2 --> ING
    W3 --> ING
    ING --> APP[Application Pods]
    APP --> PV[(Persistent Volumes)]
    WK -.metrics.-> MON[Prometheus + Grafana]
```

---

<a id="toolbox"></a>
## 🧰 DevOps Toolbox

<div align="center">

<img src="https://skillicons.dev/icons?i=terraform,ansible,kubernetes,docker,aws,gitlab,jenkins,prometheus,grafana,nginx,linux,bash,git&perline=13" alt="DevOps tools" />

<br/>

<img src="https://skillicons.dev/icons?i=python,fastapi,nodejs,express,mongodb,kafka,solidity&perline=7" alt="Development tools" />

</div>

<details>
<summary><b>📋 Full stack breakdown (click to expand)</b></summary>

<br/>

| Area | Stack |
|---|---|
| ☁️ **Cloud (AWS)** | EC2, EKS, ECS/Fargate, Lambda, VPC, IAM, S3, RDS, DynamoDB, CloudWatch, ELB/ALB, Route 53, SNS/SQS, WAF, CloudTrail |
| 🏗️ **Infrastructure as Code** | Terraform (reusable modules), Ansible |
| ☸️ **Containers & Orchestration** | Docker, Kubernetes, Helm, Ingress, RBAC, HPA, PV/PVC |
| 🔁 **CI/CD & GitOps** | GitLab CI, Jenkins (shared libraries), Argo CD |
| 📨 **Messaging & Streaming** | Apache Kafka, ActiveMQ, SNS/SQS |
| 📊 **Monitoring** | Prometheus, Grafana, AWS CloudWatch |
| 💻 **Backend** | Node.js, Express.js, Python, FastAPI, MongoDB |
| 🔗 **Blockchain** | Hyperledger Fabric, Hyperledger Besu, Solidity, IPFS |

</details>

---

## 🚀 What I Do

| | |
|---|---|
| 🏛️ **Architecture & design** | Service boundaries, API contracts, data layers, Kubernetes topology and CI/CD workflows |
| 🖥️ **Infrastructure** | HA and standard Kubernetes clusters and servers on AWS and on-premise with Terraform and Ansible |
| 🔄 **Delivery pipelines** | Helm-based releases, Argo CD GitOps and reusable Jenkins pipeline libraries |
| 🔗 **Blockchain delivery** | 10+ production apps on Hyperledger Fabric and Besu: document verification, digital identity, e-voting, supply-chain audit |
| 🎓 **Mentoring** | Design reviews and training on Kubernetes, Docker, Helm, Ansible and infrastructure automation |

---

<a id="journey"></a>
## 🧭 My Journey

```mermaid
timeline
    title Career and Education Timeline
    2016 - 2020 : B.Tech in ECE : Guru Nanak Institution Technical Campus
    2021 : Joined C-DAC as Project Engineer : DevOps and blockchain delivery
    2022 - 2024 : M.Tech in Software Engineering : BITS Pilani
    2026 : Promoted to Senior Project Engineer : Architecture and design ownership
```

---

<a id="certs"></a>
## 🏅 Certifications

<div align="center">

[![CKAD](https://img.shields.io/badge/CKAD-Certified_Kubernetes_Application_Developer-326CE5?logo=kubernetes&logoColor=white&style=for-the-badge)](https://www.credly.com/badges/ebfce6d5-e235-4207-82f9-30904af68db5)
[![Hyperledger Fabric](https://img.shields.io/badge/Hyperledger_Fabric-Certified_Practitioner-2F3134?logo=hyperledger&logoColor=white&style=for-the-badge)](https://www.credly.com/badges/9b81a7a3-294f-4f9b-bfde-67b0cc3b6bd1)
[![Besu](https://img.shields.io/badge/Besu-Certified_Professional-2F3134?logo=hyperledger&logoColor=white&style=for-the-badge)](https://www.credly.com/badges/f96ae64a-c0ba-4730-86f1-a619c6a26471/public_url)

</div>

📄 **Publication:** [Blockchain Based Digital Signature Certificate Management System](https://iaeme.com/Home/article_id/IJBT_03_02_002)  
🎓 **Education:** M.Tech in Software Engineering, BITS Pilani | B.Tech in ECE, Guru Nanak Institution Technical Campus

---

<a id="stats"></a>
## 📈 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=AmeerRiyaz&show_icons=true&include_all_commits=true&theme=radical&hide_border=true" alt="GitHub stats" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AmeerRiyaz&layout=compact&langs_count=8&theme=radical&hide_border=true" alt="Top languages" />

<img src="https://streak-stats.demolab.com/?user=AmeerRiyaz&theme=radical&hide_border=true" alt="GitHub streak" />

<img src="https://github-profile-trophy.vercel.app/?username=AmeerRiyaz&theme=radical&no-frame=true&row=1&column=7&margin-w=10" alt="GitHub trophies" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=AmeerRiyaz&theme=react-dark&hide_border=true&area=true&color=A78BFA&line=7B42BC&point=ffffff" alt="Contribution graph" width="100%" />

</div>

### 🏙️ 3D Contribution Skyline

<div align="center">

<img src="./profile-3d-contrib/profile-night-rainbow.svg" width="100%" alt="3D contribution skyline" />

</div>

### 🐍 Contribution Snake

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AmeerRiyaz/AmeerRiyaz/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AmeerRiyaz/AmeerRiyaz/output/github-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/AmeerRiyaz/AmeerRiyaz/output/github-snake.svg" />
</picture>

</div>

---

<a id="contact"></a>
## 💬 Let's Connect

<div align="center">

[![Email](https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white&style=for-the-badge)](mailto:ameerriyaz25@gmail.com)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin&logoColor=white&style=for-the-badge)](https://in.linkedin.com/in/ameer-riyaz)
[![Twitter](https://img.shields.io/badge/-Twitter-1DA1F2?logo=twitter&logoColor=white&style=for-the-badge)](https://twitter.com/AmeerRiyaz111)
[![Resume](https://img.shields.io/badge/-Resume-7B42BC?logo=adobeacrobatreader&logoColor=white&style=for-the-badge)](./Shaik_Ameer_Riyaz_Resume.pdf)

<br/>

*Infrastructure should be code, deployments should be boring, and clusters should survive a node failure.*

</div>
