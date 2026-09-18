# Laboratory 4: The Cloud-Native Engineer

## Mission Overview
As part of the Cloud-Native Engineering Team at CloudNova Technologies, this lab focused on helping a client
transition from slow, resource-heavy Virtual Machines to lightweight, fast-starting Docker containers.
The mission involved researching the architectural differences between VMs and containers, verifying a
Docker environment, deploying a live containerized Nginx web server, and documenting the full container
lifecycle for the client's IT team to replicate.

## Objectives
- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, run, manage, and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

**Checkpoint 3 — Verifying Docker**
docker --version
docker info

**Checkpoint 4 — Deploying Nginx**
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080

**Checkpoint 5 — Container Lifecycle**
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx

## Skills Learned
- How to verify a Docker installation and check daemon status.
- How to pull container images from Docker Hub.
- How port mapping (-p host:container) exposes a containerized service to the host.
- How to manage the full lifecycle of a container: list, stop, verify, and remove.
- How containerization improves resource efficiency and deployment speed compared to VMs.

## Challenges Encountered
No major issues were encountered during this lab. The KillerCoda environment came with Docker
pre-installed, and each command produced the expected output on the first try.
