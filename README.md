<div align="center">

<img src="./banner.svg" width="100%" alt="Ameer Riyaz - Senior Project Engineer, DevOps and Platform Engineering" />

<a href="https://github.com/AmeerRiyaz">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=750&height=45&lines=terraform+apply+-auto-approve;kubectl+get+nodes+%28HA+cluster+ready%29;ansible-playbook+site.yml;argocd+app+sync+production;Architecting+apps+for+government+%26+enterprise" alt="Typing SVG" />
</a>

<p align="center">
  <img src="https://img.shields.io/badge/-Terraform-7B42BC?logo=terraform&logoColor=white&style=for-the-badge" alt="Terraform" />
  <img src="https://img.shields.io/badge/-Kubernetes-326CE5?logo=kubernetes&logoColor=white&style=for-the-badge" alt="Kubernetes" />
  <img src="https://img.shields.io/badge/-AWS-232F3E?logo=amazonaws&logoColor=white&style=for-the-badge" alt="AWS" />
  <img src="https://img.shields.io/badge/-Ansible-EE0000?logo=ansible&logoColor=white&style=for-the-badge" alt="Ansible" />
  <img src="https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white&style=for-the-badge" alt="Docker" />
  <img src="https://img.shields.io/badge/-Helm-0F1689?logo=helm&logoColor=white&style=for-the-badge" alt="Helm" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=AmeerRiyaz&label=Profile+Views&color=7B42BC&style=for-the-badge" alt="Profile views" />
  <img src="https://img.shields.io/github/followers/AmeerRiyaz?label=Followers&style=for-the-badge&color=326CE5&logo=github" alt="Followers" />
  <img src="https://img.shields.io/badge/Hyderabad,_India-7B42BC?logo=googlemaps&logoColor=white&style=for-the-badge" alt="Location" />
</p>

<p align="center">
  <a href="#about"><img src="https://img.shields.io/badge/About-7B42BC?style=flat-square" alt="About" /></a>
  <a href="#pipeline"><img src="https://img.shields.io/badge/Pipeline-326CE5?style=flat-square" alt="Pipeline" /></a>
  <a href="#toolbox"><img src="https://img.shields.io/badge/Toolbox-7B42BC?style=flat-square" alt="Toolbox" /></a>
  <a href="#journey"><img src="https://img.shields.io/badge/Journey-326CE5?style=flat-square" alt="Journey" /></a>
  <a href="#certs"><img src="https://img.shields.io/badge/Certifications-7B42BC?style=flat-square" alt="Certifications" /></a>
  <a href="#stats"><img src="https://img.shields.io/badge/Stats-326CE5?style=flat-square" alt="Stats" /></a>
  <a href="#contact"><img src="https://img.shields.io/badge/Contact-7B42BC?style=flat-square" alt="Contact" /></a>
</p>

<p align="center">
  <a href="./Shaik_Ameer_Riyaz_Resume.pdf"><img src="https://img.shields.io/badge/Download-Resume_PDF-7B42BC?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Download Resume" /></a>
</p>

</div>

---

<h2 align="center"><a id="about"></a>⚙️ About Me</h2>

<p align="center">
I design, build and run distributed applications for government and enterprise clients at <b>C-DAC, Hyderabad</b>.<br/>
I own solution architecture and design, build HA and standard Kubernetes clusters on AWS and on-premise,<br/>
and automate everything with Terraform and Ansible. My domain specialty is <b>Hyperledger Fabric</b> and <b>Besu</b>.
</p>

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

<h2 align="center"><a id="pipeline"></a>🔄 How I Ship</h2>

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

<h3 align="center">⚡ Live Pipeline</h3>

<div align="center">

<img src="./pipeline.svg" width="100%" alt="Animated delivery pipeline from code to Kubernetes" />

</div>

---

<h2 align="center"><a id="toolbox"></a>🧰 DevOps Toolbox</h2>

<div align="center">

<img src="https://skillicons.dev/icons?i=terraform,ansible,kubernetes,docker,aws,gitlab,jenkins,prometheus,grafana,nginx,linux,bash,git&perline=13" alt="DevOps tools" />

<br/><br/>

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

<h2 align="center">🚀 What I Do</h2>

| Focus | Details |
|---|---|
| 🏛️ **Architecture & design** | Service boundaries, API contracts, data layers, Kubernetes topology and CI/CD workflows |
| 🖥️ **Infrastructure** | HA and standard Kubernetes clusters and servers on AWS and on-premise with Terraform and Ansible |
| 🔄 **Delivery pipelines** | Helm-based releases, Argo CD GitOps and reusable Jenkins pipeline libraries |
| 🔗 **Blockchain delivery** | 10+ production apps on Hyperledger Fabric and Besu: document verification, digital identity, e-voting, supply-chain audit |
| 🎓 **Mentoring** | Design reviews and training on Kubernetes, Docker, Helm, Ansible and infrastructure automation |

---

<h2 align="center"><a id="journey"></a>🧭 My Journey</h2>

```mermaid
timeline
    title Career and Education Timeline
    2016 - 2020 : B.Tech in ECE : Guru Nanak Institution Technical Campus
    2021 : Joined C-DAC as Project Engineer : DevOps and blockchain delivery
    2022 - 2024 : M.Tech in Software Engineering : BITS Pilani
    2026 : Promoted to Senior Project Engineer : Architecture and design ownership
```

---

<h2 align="center"><a id="certs"></a>🏅 Certifications</h2>

<p align="center">
  <a href="https://www.credly.com/badges/ebfce6d5-e235-4207-82f9-30904af68db5"><img src="https://img.shields.io/badge/CKAD-Certified_Kubernetes_Application_Developer-326CE5?logo=kubernetes&logoColor=white&style=for-the-badge" alt="CKAD" /></a>
  <a href="https://www.credly.com/badges/9b81a7a3-294f-4f9b-bfde-67b0cc3b6bd1"><img src="https://img.shields.io/badge/Hyperledger_Fabric-Certified_Practitioner-2F3134?logo=hyperledger&logoColor=white&style=for-the-badge" alt="Hyperledger Fabric" /></a>
  <a href="https://www.credly.com/badges/f96ae64a-c0ba-4730-86f1-a619c6a26471/public_url"><img src="https://img.shields.io/badge/Besu-Certified_Professional-2F3134?logo=hyperledger&logoColor=white&style=for-the-badge" alt="Besu" /></a>
</p>

<p align="center">
📄 <b>Publication:</b> <a href="https://iaeme.com/Home/article_id/IJBT_03_02_002">Blockchain Based Digital Signature Certificate Management System</a><br/>
🎓 <b>Education:</b> M.Tech in Software Engineering, BITS Pilani | B.Tech in ECE, Guru Nanak Institution Technical Campus
</p>

---

<h2 align="center"><a id="stats"></a>📈 GitHub Stats</h2>

<p align="center">
  <img height="180" src="https://github-readme-stats.vercel.app/api?username=AmeerRiyaz&show_icons=true&include_all_commits=true&theme=radical&hide_border=true" alt="GitHub stats" />
  <img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AmeerRiyaz&layout=compact&langs_count=8&theme=radical&hide_border=true" alt="Top languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=AmeerRiyaz&theme=radical&hide_border=true" alt="GitHub streak" />
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=AmeerRiyaz&theme=radical&no-frame=true&row=1&column=7&margin-w=10" alt="GitHub trophies" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=AmeerRiyaz&theme=react-dark&hide_border=true&area=true&color=A78BFA&line=7B42BC&point=ffffff" alt="Contribution graph" width="100%" />
</p>

<!-- <h3 align="center">🏙️ 3D Contribution Skyline</h3>

<p align="center">
  <img src="./profile-3d-contrib/profile-night-rainbow.svg" width="100%" alt="3D contribution skyline" />
</p> -->

<h3 align="center">🐍 Contribution Snake</h3>

<p align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AmeerRiyaz/AmeerRiyaz/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AmeerRiyaz/AmeerRiyaz/output/github-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/AmeerRiyaz/AmeerRiyaz/output/github-snake.svg" />
</picture>
</p>

---

<h2 align="center"><a id="contact"></a>💬 Let's Connect</h2>

<p align="center">
  <a href="mailto:ameerriyaz25@gmail.com"><img src="https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white&style=for-the-badge" alt="Email" /></a>
  <a href="https://in.linkedin.com/in/ameer-riyaz"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin&logoColor=white&style=for-the-badge" alt="LinkedIn" /></a>
  <a href="https://twitter.com/AmeerRiyaz111"><img src="https://img.shields.io/badge/-Twitter-1DA1F2?logo=twitter&logoColor=white&style=for-the-badge" alt="Twitter" /></a>
  <a href="./Shaik_Ameer_Riyaz_Resume.pdf"><img src="https://img.shields.io/badge/-Resume-7B42BC?logo=adobeacrobatreader&logoColor=white&style=for-the-badge" alt="Resume" /></a>
</p>

<p align="center"><i>Infrastructure should be code, deployments should be boring, and clusters should survive a node failure.</i></p>
