# Laboratory 3 – Multi-Cloud Explorer

Cloud Evaluation Team mission for CloudNova Technologies: researching AWS, Azure,
and GCP, comparing their services, and recommending platforms for client scenarios.

## Contents
- `aws-research.md` – AWS overview and core services
- `azure-research.md` – Azure overview and core services
- `gcp-research.md` – GCP overview and core services
- `cloud-platform-comparison.md` – Comparison and service-matching tables
- `client-recommendations.md` – Recommendations for Clients A–D + decision matrix
- `reflection.md` – Mission reflection
- `screenshots/` – Evidence for each checkpoint

## Checkpoint 7 – Linux Investigation

**Operating System:** Ubuntu 24.04.4 LTS, Kernel 6.8.0-138-generic, x86_64 architecture, running as a KVM virtual machine

**CPU:** 1 vCPU, Intel Xeon E312xx (Sandy Bridge), x86_64, 1 socket / 1 core / 1 thread, 16 MiB L3 cache

**Memory:** 1.9Gi total, 817Mi free, 1.4Gi available, 1.0Gi swap

**Disk Space:** 19G total on root (`/dev/vda1`), 5.4G used, 13G available (30% used)

### If this Linux server were migrated to the cloud, which AWS, Azure, and GCP services could host it?

Given the small footprint of this server (1 vCPU, ~2GB RAM, ~19GB disk), it maps to the smallest general-purpose instance tiers across all three providers:

- **AWS:** Amazon EC2, `t3.micro` or `t3.small` instance type (1–2 vCPUs, 1–2GB RAM), paired with Amazon EBS (General Purpose SSD, ~20GB volume) for the root disk.
- **Azure:** Azure Virtual Machines, `B1s` or `B1ms` size (burstable, 1 vCPU, 1–2GB RAM), paired with Azure Managed Disks (Standard SSD, ~20GB).
- **GCP:** Compute Engine, `e2-micro` or `e2-small` machine type (1–2 vCPUs, 1–2GB RAM), paired with a Persistent Disk (Standard or Balanced, ~20GB).

[Add 2–3 sentences here in your own words on which one you'd personally pick for this server and why.]

### Terminal Evidence

**Operating System check:**

![OS screenshot](./screenshots/os-screenshot.png)

**CPU information:**

![CPU screenshot](./screenshots/cpu-screenshot.png)

**Memory information:**

![Memory screenshot](./screenshots/memory-screenshot.png)

**Disk space:**

![Disk screenshot](./screenshots/disk-screenshot.png)
