Laboratory 02 – Build the Cloud Infrastructure Blueprint

Mission Overview
This laboratory activity simulates the planning phase of a cloud deployment for a fictional company, CloudNova Technologies. Using a Linux server provisioned through the KillerCoda Playground, I investigated the underlying infrastructure, identified its major components, compared how the top three public cloud providers offer equivalent services, and designed a simple cloud architecture diagram — all documented as a Cloud Infrastructure Assessment Report.

Objectives
- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

Cloud Infrastructure Components
- Compute – The processing power (CPU/RAM) that runs applications and workloads. Investigated using `lscpu` and `free -h` on the KillerCoda server.
- Storage – Where data is stored persistently or temporarily. Investigated using `df -h`, showing partitions like `/dev/vda1` mounted at `/`.
- Networking – Enables communication between systems and the internet. Investigated using `ip a`, revealing the server's private IP and network interfaces.
- Operating System – Manages hardware and provides the runtime environment. The server runs Ubuntu 24.04.4 LTS, confirmed via `cat /etc/os-release`.

Full details are documented in `cloud-components.md` and `infrastructure-report.md`.

Tools Used
- KillerCoda Playground (Linux terminal sandbox)
- Git and GitHub (version control and portfolio hosting)
- Markdown (documentation formatting)
- Draw.io (cloud architecture diagram)

Linux Commands Executed
| Command | Purpose |
|---|---|
| `cat /etc/os-release` | Identify the operating system |
| `uname -r` | Check kernel version |
| `lscpu` | View CPU model and core count |
| `free -h` | Check total RAM |
| `df -h` | Check disk capacity and mounted filesystems |
| `hostname` | Get the server hostname |
| `ip a` | View network interfaces and IP address |

Skills Learned
- How to inspect a Linux server's hardware and software resources from the command line.
- How to map real Linux system components (CPU, disk, network interfaces) to cloud infrastructure concepts (compute, storage, networking).
- How to compare equivalent services across AWS, Azure, and GCP.
- How to design a basic cloud architecture diagram and export it for documentation.
- How to write clear, structured technical documentation using Markdown.

Challenges Encountered
- Initially had trouble committing changes to Git due to a missing user identity configuration (`user.name` and `user.email`), which had to be reconfigured after the KillerCoda session reset.
- Needed to switch from password-based GitHub authentication to a Personal Access Token (PAT), since GitHub no longer accepts plain passwords for terminal-based pushes.
- Had to double-check `git status` and `git log` carefully to confirm whether changes were actually staged, committed, and pushed, since a forgotten `commit` step silently left files unpushed.
