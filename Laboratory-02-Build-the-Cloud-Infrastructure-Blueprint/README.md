# Laboratory 02 — Build the Cloud Infrastructure Blueprint

## Mission Overview
This lab investigates the components of cloud infrastructure by inspecting a Linux server running in a KillerCoda cloud environment, documenting the findings as if preparing a Cloud Infrastructure Assessment Report for a client.

## Objectives
- Explain the major components of cloud infrastructure.
- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

## Cloud Infrastructure Components
Investigated and documented four core components on the KillerCoda server — compute (CPU/cores), storage (disks and mounted filesystems), networking (hostname/IP), and the operating system (Ubuntu 24.04.4 LTS) — with details in `infrastructure-report.md` and `cloud-components.md`. Also compared how AWS, Azure, and GCP each offer equivalent versions of these components in `cloud-provider-comparison.md`.

## Tools Used
- KillerCoda Playground (Ubuntu 24.04 server)
- Git / GitHub (version control and portfolio hosting)
- [diagramming tool used — Draw.io / Excalidraw / PowerPoint]

## Linux Commands Executed
```bash
cat /etc/os-release
uname -r
lscpu
free -h
df -h
mount | column -t
hostname
hostname -I
```

## Skills Learned
- Reading a Linux server's hardware and software profile directly from the terminal
- Telling apart compute, storage, networking, and the OS as separate layers of infrastructure
- Matching up equivalent cloud services across AWS, Azure, and GCP
- Managing a technical portfolio through Git — cloning, staging, committing, pushing, and pulling
- Putting together structured technical documentation in Markdown

## Challenges Encountered
- Ran the initial `mkdir`/`git add`/`commit`/`push` sequence in a fresh KillerCoda playground before cloning the repo, hitting `fatal: not a git repository` — fixed by cloning the existing GitHub repo first and working from inside it
- The first `git commit` failed silently with `Author identity unknown` — fixed by running `git config --global user.email` and `user.name` before retrying
- GitHub rejected the account password when `git push` prompted for one — had to generate a Personal Access Token (with Contents: Read and write permission) and use that instead
- Uploading screenshots directly through GitHub's drag-and-drop screen made them hard to rename into the `screenshots/` folder — worked around it by committing the files first, then renaming/moving each one afterward through the file editor
