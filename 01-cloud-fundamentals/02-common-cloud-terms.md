# Cloud Computing Vocabulary

This document explains key terms used in cloud computing and how they relate to real-world cloud systems.

---

## Virtualization

Virtualization is the process of creating a virtual version of computing resources such as servers, storage, or networks.

It allows multiple virtual machines to run on a single physical machine by sharing underlying hardware resources.

---

## Virtual Machine (VM)

A Virtual Machine is a software-based computer that behaves like a physical machine.

It runs an operating system and applications independently, but shares physical hardware with other VMs.

Example: Google Compute Engine VM in GCP.

---

## API (Application Programming Interface)

An API is a set of rules that allows software systems to communicate.

In cloud computing, APIs are used to:

- create resources (VMs, storage buckets)
- manage services
- automate infrastructure

Example: GCP REST APIs or `gcloud` CLI commands.

---

## Region

A region is a geographic location where cloud infrastructure is hosted.

Each region is an independent area containing multiple data centers.

Example:

- `us-central1` (Iowa, USA)
- `europe-west1` (Belgium)

---

## Availability Zone (Zone)

A zone is an isolated location within a region.

Each zone has independent power, cooling, and networking to reduce failure risk.

Example:

- `us-central1-a`
- `us-central1-b`

---

## Scalability

Scalability is the ability of a system to handle increased workload by adding resources.

Types:

- Vertical scaling: increasing power of a single machine
- Horizontal scaling: adding more machines (preferred in cloud)

---

## Elasticity

Elasticity is the ability of a system to automatically scale resources up or down based on demand.

Example:

- traffic increases → more servers added automatically
- traffic drops → resources removed to save cost

---

## Agility

Agility refers to the ability to quickly deploy and modify infrastructure and applications.

Cloud enables agility by allowing resources to be created in minutes instead of weeks.

---

## High Availability (HA)

High Availability means a system is designed to remain operational even when components fail.

Typical design includes:

- multiple zones
- load balancing
- redundant systems

---

## Fault Tolerance

Fault tolerance is the ability of a system to continue functioning even when part of it fails.

Difference from HA:

- HA = keeps system available
- Fault tolerance = continues running without interruption

---

## Disaster Recovery (DR)

Disaster recovery refers to restoring systems and data after a major failure or disaster.

It includes:

- backups
- failover systems
- recovery plans

---

## Load Balancing

Load balancing distributes incoming traffic across multiple servers.

Benefits:

- prevents overload
- improves performance
- increases availability

Example: Google Cloud Load Balancer.

---

## Container

A container is a lightweight, portable environment that packages an application and its dependencies.

Unlike VMs, containers share the host OS kernel.

Example: Docker containers.

---

## Kubernetes

Kubernetes is a system for managing and scaling containers automatically.

It handles:

- deployment
- scaling
- load balancing
- self-healing of containers

Example: Google Kubernetes Engine (GKE)

---

## IAM (Identity and Access Management)

IAM controls who can access cloud resources and what actions they can perform.

It uses:

- users
- roles
- permissions

Example:
A user can be allowed to start VMs but not delete projects.

---

## Storage Types

Cloud storage is categorized into:

- Object storage (e.g., Cloud Storage)
- Block storage (e.g., Persistent Disks)
- File storage (e.g., Filestore)

---

## Summary

Cloud computing is built around:

- Virtualized infrastructure
- Automated scaling
- Distributed systems
- Security through IAM
- API-driven management
