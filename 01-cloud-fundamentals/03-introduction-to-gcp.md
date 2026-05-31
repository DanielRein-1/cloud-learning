# Introduction to Cloud and GCP

---

## 1. Cloud Computing Definition

Cloud computing is the on-demand delivery of compute, storage, networking, and platform services over the internet with:

- elastic scaling
- pay-as-you-go pricing
- globally distributed infrastructure

These resources are provisioned and managed through APIs or cloud consoles instead of physical hardware management.

---

## 2. Core Cloud Architecture Model

All cloud platforms (GCP, AWS, Azure) are built on three foundational layers:

### Compute Layer

Executes workloads:

- Virtual Machines (VMs)
- Containers
- Serverless compute

### Storage Layer

Persistent data systems:

- Object storage
- Block storage
- Managed databases

### Networking Layer

Interconnects resources:

- Virtual networks (VPC)
- Routing
- Load balancing
- DNS services

---

## 3. Cloud Service Models

### IaaS (Infrastructure as a Service)

Provides virtualized compute resources.

User manages:

- OS
- runtime
- applications

Provider manages:

- hardware
- virtualization

Example:

- Google Compute Engine

---

### PaaS (Platform as a Service)

Provides managed runtime environment.

User manages:

- application code

Provider manages:

- OS
- runtime
- scaling

Example:

- Google App Engine
- Cloud Run

---

### SaaS (Software as a Service)

Fully managed applications delivered over the internet.

User only consumes software.

Example:

- Gmail
- Google Drive

---

## 4. Traditional IT vs Cloud Model

| Traditional Infrastructure   | Cloud Infrastructure            |
| ---------------------------- | ------------------------------- |
| Fixed capacity hardware      | On-demand provisioning          |
| Manual scaling               | Auto-scaling systems            |
| High upfront cost            | Operational expenditure         |
| Single location              | Multi-region distribution       |
| Hardware management required | Provider-managed infrastructure |

---

## 5. Google Cloud Platform (GCP)

GCP is Google’s cloud computing platform built on the same infrastructure that powers:

- Google Search
- YouTube
- Gmail
- Maps

It provides global-scale distributed systems for compute, storage, networking, and data processing.

---

## 6. Core GCP Service Domains

### Compute Services

- Compute Engine (VMs)
- Google Kubernetes Engine (GKE)
- Cloud Run (serverless containers)
- App Engine (PaaS)

---

### Storage Services

- Cloud Storage (object storage)
- Persistent Disk (block storage)

---

### Database Services

- Cloud SQL (relational databases)
- Firestore (NoSQL)
- BigQuery (analytics warehouse)

---

### Networking Services

- Virtual Private Cloud (VPC)
- Cloud Load Balancing
- Cloud DNS
- Cloud CDN

---

### Identity & Security (IAM)

Identity and Access Management controls:

- authentication (who you are)
- authorization (what you can do)

Key components:

- users
- service accounts
- roles
- policies

---

## 7. Cloud Shell Environment

Cloud Shell is a managed Linux environment provided by GCP with:

- preinstalled CLI tools (gcloud, kubectl, git)
- ephemeral compute environment
- authenticated access to GCP projects

---

## 8. VM Provisioning Model (Critical Concept)

When a VM is created in GCP:

1. API request is sent to Compute Engine
2. Scheduler selects physical host in a region/zone
3. Hypervisor allocates isolated virtual machine
4. Boot disk is attached and OS is initialized
5. Network interface is assigned (VPC + IP)

Result: a fully isolated compute instance running on shared physical infrastructure.

---

## 9. Application Deployment Flow

Typical cloud deployment pipeline:

1. Source code is built into artifact/container image
2. Artifact stored in registry
3. Compute service pulls image
4. Application runs in VM/container/serverless runtime
5. Traffic is exposed via load balancer or ingress

---

## 10. Essential GCP CLI Commands

```bash
gcloud auth list
gcloud config list
gcloud projects list
gcloud compute instances list
