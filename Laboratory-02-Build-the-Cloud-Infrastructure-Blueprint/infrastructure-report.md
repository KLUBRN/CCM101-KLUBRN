# Cloud Infrastructure Assessment Report

Findings from investigating the KillerCoda Linux server using standard Linux diagnostic commands.

| Item | Command used | Finding |
|---|---|---|
| Operating System | `cat /etc/os-release` | Ubuntu 24.04.4 LTS (Noble Numbat) |
| Kernel Version | `uname -r` | 6.8.0-138-generic |
| CPU Model | `lscpu` | Intel Xeon E312xx (Sandy Bridge), x86_64 architecture |
| CPU Cores | `lscpu` / `nproc` | 1 core (1 socket, 1 core per socket, 1 thread per core) |
| Total RAM | `free -h` | 1.9Gi total, 828Mi free |
| Disk Capacity | `df -h` | 19G main volume (`/dev/vda1`), 5.4G used, 13G available (30% used) |
| Mounted File Systems | `mount \| column -t` | `/dev/vda1` (ext4) at `/`, `/dev/vda16` (ext4) at `/boot`, `/dev/vda15` (vfat) at `/boot/efi`, plus virtual filesystems (`tmpfs`, `proc`, `sysfs`, `cgroup2`, etc.) used internally by Linux |
| Hostname | `hostname` | ubuntu |
| IP Address | `hostname -I` | 173.30.1.2 (container network), 172.17.0.1 (Docker bridge) |

Screenshots of each command's output are saved in `screenshots/` (`server-information.png`, `storage-information.png`, `network-information.png`).
