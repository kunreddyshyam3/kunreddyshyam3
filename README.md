# 👋 Hi, I'm Shyamsunder Reddy

<img src="https://media.giphy.com/media/HscDLzkO8EOTmgkhQP/giphy.gif" width="200" align="right">

Platform & infrastructure engineer with **5+ years** across DevOps, SRE, and platform engineering — three names for the same job at different companies.

These days I run a multi-tenant **OpenShift** platform that **300+ production applications** ship on, built on **IBM Power (ppc64le)**. Most of my work lives in the gap between "it deploys" and "it's actually reliable": build pipelines, observability that answers questions instead of generating noise, and turning one-off requests into platform capabilities.

## 🚀 Quick Facts

- 🔭 Currently a **Platform / Infrastructure Engineer at IBM** (India Systems Development Labs, Hyderabad)
- 🛠️ Day job: OpenShift fleet ops, Terraform, Helm, CI/CD, Prometheus/Thanos, and porting workloads to Power where no upstream image exists
- 🌱 Currently deep in **agentic AI for operations** — MCP servers, safety guardrails, and whether an LLM can be trusted near a live cluster
- 🎯 Working toward contributing to **CNCF projects**
- ⚡ Fun fact: the most interesting bug I've found this year wasn't in the code — it was the kubelet silently rotating away 80% of my telemetry data

## 🔨 What I'm Building

**[Belay](https://github.com/kunreddyshyam3)** — guardrails for agent-driven infrastructure
An MCP-native layer that sits between an LLM agent and a live cluster, enforcing `scope` → `dry` → `run` → `undo` before any generated command executes. *terraform plan before apply, for agentic ops.* Integrated with IBM BOB and the OpenShift MCP server. 🏆 **IBM Bobathon Innovator**

**PromQL telemetry collector** — observability without object storage
Built when a Loki deployment turned out to be infeasible on an all-Power cluster with no ODF. 24 validated network queries, rolling six-hour windows, ~236K samples per run. Surfaced two production faults the default alerting stack never fired on.

**ppc64le workload enablement** — making an architecture a viable target
Container images for MongoDB Enterprise, IBM MQ, and a Next.js app that needed its SWC native binary compiled from Rust source, because upstream ppc64le artifacts don't exist.

## 🛠️ Tech Stack

**Orchestration & Containers**
<p>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
  <img src="https://img.shields.io/badge/OpenShift-EE0000?style=for-the-badge&logo=redhatopenshift&logoColor=white" alt="OpenShift"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white" alt="Helm"/>
</p>

**Infrastructure as Code**
<p>
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white" alt="Terraform"/>
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white" alt="Ansible"/>
  <img src="https://img.shields.io/badge/Vault-FFEC6E?style=for-the-badge&logo=vault&logoColor=black" alt="Vault"/>
</p>

**CI/CD**
<p>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white" alt="Jenkins"/>
  <img src="https://img.shields.io/badge/Azure_DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white" alt="Azure DevOps"/>
</p>

**Observability**
<p>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white" alt="Prometheus"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Grafana"/>
  <img src="https://img.shields.io/badge/Loki-F46800?style=for-the-badge&logo=grafana&logoColor=white" alt="Loki"/>
  <img src="https://img.shields.io/badge/OpenTelemetry-425CC7?style=for-the-badge&logo=opentelemetry&logoColor=white" alt="OpenTelemetry"/>
</p>

**Cloud & Languages**
<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Azure"/>
  <img src="https://img.shields.io/badge/IBM_Power-052FAD?style=for-the-badge&logo=ibm&logoColor=white" alt="IBM Power"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash"/>
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go"/>
</p>

## 🏆 Selected Wins

- **200%** higher build parallelism and **45%** faster builds — rebuilt Gradle build infrastructure on Kubernetes for silicon-engineering teams
- **65%** smaller telemetry payload (26.7 MB → 9.28 MB per run) — after tracing silent data loss to the kubelet's 50 MiB log-rotation ceiling, not to the queries
- **60%** faster provisioning and **30%** higher resource utilization — IaC-driven automation across Kubernetes and oVirt
- **40%** lower MTTR — highly available Prometheus/Grafana with alerting tuned for proactive detection
- **99.99%** uptime — PostgreSQL high availability on Kubernetes, with failover testing and backup verification

## ✍️ Writing

- [Architecture of Kubernetes](https://kubernetesfirstbest.hashnode.dev/architecture-of-kubernetes)
- [Deep Dive into Kubernetes](https://kubernetesfirstbest.hashnode.dev/)
- [CI/CD Pipeline Mastery](https://devopscommunity.hashnode.dev/cicd)
- [Docker Demystified](https://docker01.hashnode.dev/docker)

## 📊 GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kunreddyshyam3&show_icons=true&hide_border=true&theme=tokyonight" alt="GitHub stats" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kunreddyshyam3&layout=compact&hide_border=true&theme=tokyonight" alt="Top languages" height="165"/>
</p>

## 📫 Let's Connect

<p>
  <a href="https://linkedin.com/in/shyamkunreddy">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:ssrkunreddy@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"/>
  </a>
  <a href="https://www.credly.com/users/shyamsunder-reddy">
    <img src="https://img.shields.io/badge/Credly-FF6B00?style=for-the-badge&logo=credly&logoColor=white" alt="Credly"/>
  </a>
</p>

<sub>Open to conversations about platform engineering, SRE, and where agentic AI actually belongs in ops.</sub>
