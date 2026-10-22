# Final Reflection: Mission 1 to Mission 10

**Student:** Sandy Charles A. Mediana
**Course:** CCM101 - Cloud Computing

## 1. Where I Started
Before Mission 1, I had never used the Linux terminal, and I thought cloud computing only meant storing files online.

## 2. My Journey
- **Missions 1-3 (Welcome to the Cloud, Build the Cloud Infrastructure, Multi-Cloud Explorer):** I learned what cloud computing is, how infrastructure is built, and how different cloud providers compare.
- **Missions 4-6 (Cloud Native, Cloud Data, Cloud Deployment):** I learned to use Docker containers, work with persistent data, and deploy applications.
- **Missions 7-9 (Cloud Operations, Cloud Security, Cloud Automation):** I learned monitoring, firewall security, and Bash scripting with scheduled tasks.
- **Mission 10 (Enterprise Cloud Architect):** I designed and deployed a WordPress + MariaDB stack with Docker Compose, secured it with UFW (default deny), and automated database backups with a Bash script and cron.

## 3. Challenges and How I Solved Them
- **Git push confusion:** My Lab 10 folder did not appear on GitHub because Git does not track empty folders. I fixed it by adding a file, committing, and pushing.
- **Overwritten README:** I accidentally overwrote the root README.md because I ran my command in the wrong folder. I used `git show --stat HEAD` to find the problem and `git checkout HEAD~1 -- README.md` to restore it. Lesson: always check the terminal path before running commands.
- **Docker and the firewall:** I learned that Docker publishes ports by editing iptables directly, so a UFW rule alone may not control access to a container port. I solved this by keeping the database container without any published ports, so only the WordPress port is reachable from outside. Lesson: always test the firewall from outside instead of trusting the rules alone.

## 4. Key Lessons
1. Infrastructure as Code (docker-compose.yml) makes deployments repeatable.
2. Security must be built in from the start: default deny, only necessary ports open.
3. Backups and automation protect a system when something goes wrong.

## 5. How Chapters 1-9 Connect in My Final Project
Virtualization provides the Ubuntu Server foundation. Containers run the WordPress and MariaDB tiers. Persistent volumes keep data after a reboot. UFW secures the host, and Bash with cron keeps backups running without manual work.

## 6. What I Would Improve
With more time, I would add HTTPS, monitoring and alerts, and off-site backups.

## 7. Final Thoughts
At the start, I saw cloud computing as a place to store files online. Now I see it as a set of connected tools for building, securing, and automating real systems. Mission 10 showed me that I can design and deploy a complete infrastructure without step-by-step instructions, and the part I am most proud of is making the system secure and able to back itself up.
