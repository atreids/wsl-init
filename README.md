# Overview

This repo holds setup instructions and scripts for a fresh WSL installation.

## WSL Initial Setup

Relevant notes:

- Admin permission is required for WSL installation.
- HyperV should be enabled.
- WSL installations are per-user.

powershell:

```powershell
> wsl --update
> wsl --install
```

WSL will install the default distribution which is Ubuntu. You will need to create a Linux user.

## Git installation

Install Git.

```bash
sudo apt-get install git
```

## Generate SSH key

Generate key

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Add key to your Github account.

## Clone this repo

```bash
git clone git@github.com:atreids/wsl-init.git
```

## Init script

Run script to setup WSL installation.

```bash
./wsl-init.sh
```
