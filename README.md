# GCP Labs — Cloud Security Learning Journal

**Martin Neizer** | CCNA Certified | Google Associate Cloud Engineer (in progress)  
Seeking remote work in cloud security and cloud infrastructure

---

## About This Repository

This repository documents my hands-on GCP learning journey — building, breaking, and securing real cloud infrastructure from scratch. Each week covers a new set of services and security concepts, with daily lab notes, screenshots, and honest reflections on what worked and what confused me.

My focus is on the **security layer of cloud infrastructure**: identity and access management, least-privilege design, secrets management, service account hardening, and secure networking patterns.

---

## Skills Demonstrated

| Area | Topics Covered |
|---|---|
| **Networking** | VPCs, subnets, firewall rules, internal/external load balancers, Cloud Armor |
| **Compute** | GCE VMs, managed instance groups (MIGs), auto-healing, instance templates |
| **IAM & Identity** | IAM roles, conditional bindings, temporary access windows, service account impersonation |
| **Containers** | GKE clusters, Workload Identity, Kubernetes service accounts, pod authentication |
| **Serverless** | Cloud Run, Cloud Functions, Eventarc, Pub/Sub triggers |
| **Databases** | Cloud SQL (MySQL), Secret Manager integration, serverless-to-database pipelines |
| **Security Patterns** | Least-privilege IAM, no long-lived key files (Workload Identity), secrets-as-env-vars, zero-trust access windows |
| **CLI & Tooling** | gcloud CLI, kubectl, Cloud Console, dependency-aware teardown |

---

## Weekly Lab Index

### [Week 01 — GCP Foundations & Networking](./week-01-foundations)
Networking fundamentals, GCP VPCs, subnets, VM deployment, SSH access, and basic firewall rules.

### [Week 02 — Compute & Firewalls](./week-02-foundations)
Deploying Flask apps on GCE, firewall hardening, network tags, and CLI-based VPC management.

### [Week 03 — Managed Instance Groups & Load Balancing](./week-03-foundations)
Instance templates, MIGs, auto-healing (chaos testing), internal load balancers, and dependency teardown order.

### [Week 04 — Cloud Armor & IAM Hardening](./week-04-foundations)
Cloud Armor security policies, WAF-style rules, IAM identity hardening, and least-privilege role assignments.

### [Week 05 — Advanced IAM & Cloud Run](./week-05-foundations)
IAM conditional bindings, time-based access windows, service account impersonation, and Cloud Run deployments.

### [Week 06 — Serverless & Pub/Sub](./week-06-foundations)
Cloud Functions, Pub/Sub messaging, Eventarc triggers, and serverless pipeline architecture.

### [Week 07 — Cloud SQL & Secret Manager](./week-07-foundations)
Pub/Sub → Cloud Function → Cloud SQL pipeline. Secret Manager for credential handling. Secure serverless-to-database patterns.

### [Week 08 — GKE & Workload Identity](./week-08-foundations)
GKE cluster setup, Kubernetes service accounts (KSA), GCP service accounts (GSA), Workload Identity binding — end-to-end authentication without key files.

---

## Highlighted Labs

- **[GKE Workload Identity](./week-08-foundations/w8-day1-labs/GKE-WLI)** — Full KSA → GSA → IAM binding chain proven via pod logs. No key files.
- - **[IAM Temporary Access Windows](./week-05-foundations/day-02-temporary-access/day-02-w5-labs)** — Time-based conditional IAM bindings, impersonation, and clean removal.
  - - **[Pub/Sub to Cloud SQL Pipeline](./week-07-foundations/SQL-logs/pubToSQL)** — Serverless event pipeline with Secret Manager credential injection.
    - - **[Managed Instance Group & Auto-Healing](./week-03-foundations/day-01-w3-labs/day-01-mig)** — Chaos testing: manual VM deletion and observed MIG self-healing within seconds.
      - - **[Cloud Armor Security Policy](./week-04-foundations/day-01-w4-labs/day-01-cloudarmor)** — WAF-style rules and IP-based access control at the load balancer level.
       
        - ---

        ## Certifications

        - **CCNA** — Cisco Certified Network Associate (networking fundamentals, TCP/IP, routing & switching)
        - - **Google Associate Cloud Engineer** — In progress
         
          - ---

          ## Goals

          I am building toward a remote role in **cloud security**, cloud infrastructure, or DevSecOps. This repository is a live record of my learning — updated weekly as I progress toward my ACE certification and beyond.

          Open to junior/mid-level remote opportunities in: cloud security engineering, GCP infrastructure, IAM/identity, or cloud operations.

          ---

          *Last updated: May 2026*
