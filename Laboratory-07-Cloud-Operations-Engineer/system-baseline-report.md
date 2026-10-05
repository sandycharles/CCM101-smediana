# System Baseline Report

## Host Resources

| Resource | Value |
|---|---|
| Total RAM | 1.9 GiB |
| Root (/) storage capacity | 19 GB |

## Memory Snapshot (free -h)

- Used: 423 MiB
- Free: 1.1 GiB
- Available: 1.4 GiB

## Disk Snapshot (df -h)

- Filesystem: /dev/vda1
- Size: 19 GB
- Used: 5.4 GB (30%)
- Available: 13 GB

## Why Disk Space Matters Before a Traffic Surge

Checking disk space is critical before a traffic surge because thousands of visitors generate large amounts of logs and cached data, and if the disk becomes full, the web server can fail to write data and crash or stop serving users.

## Evidence

- screenshots/memory-check.png
- screenshots/disk-check.png
