# Cloud Infrastructure Components

## Compute Resources
**What it is:** The part of the computer that does the actual work — running programs and processing instructions.

**On this server:** 1 vCPU (Intel Xeon E312xx, Sandy Bridge) — this is the part doing all the processing in this environment.

**Why it matters in cloud computing:** Compute is basically what you're paying a cloud provider for — it's the "engine" that runs everything. Unlike a physical computer with fixed hardware, cloud compute can grow or shrink on demand — you can go from 1 processor to hundreds whenever you need to.

## Storage Resources
**What it is:** Where files, data, and the operating system are saved.

**On this server:** A 19GB disk (`/dev/vda1`) holding the main filesystem, plus two smaller sections for boot files (`/boot` and `/boot/efi`).

**Why it matters in cloud computing:** Storage needs to keep working even if the server itself is turned off or replaced. In the cloud, storage can be added, removed, or resized on its own, separate from the server — which matters a lot for backups and recovering from failures.

## Networking Resources
**What it is:** What lets the server talk to other computers and the internet.

**On this server:** Hostname `ubuntu`, with an internal IP address (`173.30.1.2`) and a second address (`172.17.0.1`) used for Docker's internal networking.

**Why it matters in cloud computing:** Without networking, a server would be isolated — no one could reach it and it couldn't reach anything else. Cloud networking tools (like VPCs and firewalls) control who and what is allowed to connect.

## Operating System
**What it is:** The software that manages the hardware and lets other programs run on top of it.

**On this server:** Ubuntu 24.04.4 LTS (Noble Numbat), kernel 6.8.0-138-generic.

**Why it matters in cloud computing:** The OS is the layer between the raw machine and the tools you actually use. Cloud providers let you pick from many operating systems as a starting template, so you can choose whichever one fits what you're building.
