# Skill 01: VPS Baseline

## Goal

Prepare a clean Linux VPS for an AI operations runtime.

## Recommended starting point

A current Ubuntu or Debian based VPS is a common choice for this workflow. Check the current Hermes Agent platform documentation before choosing an image.

## Basic host check

Run:

```bash
uname -a
cat /etc/os-release
free -h
df -h
nproc
timedatectl
```

Record the VPS facts in `templates/VPS-INVENTORY.md`.

## Install the basic prerequisites

For Ubuntu or Debian:

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install -y git curl xz-utils
```

If your chosen Hermes features need native build tools, also install:

```bash
sudo apt install -y build-essential
```

## Functional acceptance

Confirm these commands return successfully:

```bash
git --version
curl --version
xz --version
```

When the host is stable and the prerequisites are available, continue to Skill 02.
