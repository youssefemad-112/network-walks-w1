# network-walks-w1
This repository documents the process of setting up a Kali Linux virtual machine for penetration testing and security analysis as my first task during my internship at Network Walks.
# Kali Linux Lab Setup - VirtualBox
**network-walks Internship - Task 1**

## 📝 Objective
This repository documents the step-by-step process of setting up a secure and isolated **Kali Linux** virtual machine using **VirtualBox**. This foundational setup is my first task as a Cybersecurity Intern at **network-walks**, preparing the environment for future penetration testing and security analysis labs.

## 🛠️ Prerequisites
Before starting, ensure you have downloaded the following:
1. [Oracle VM VirtualBox](https://www.virtualbox.org/wiki/Downloads)
2. [Kali Linux Pre-built VM Image](https://www.kali.org/get-kali/#kali-virtual-machines) (VirtualBox 64-bit version)

## ⚙️ Virtual Machine Configuration
To ensure smooth performance during security testing, the VM is configured with the following hardware allocations:
* **Operating System:** Linux (Debian 64-bit)
* **RAM:** 4096 MB (4 GB)
* **Processors (CPU):** 2 Cores
* **Network Adapter:** NAT (To allow internet access inside the isolated VM)

---

## 🚀 Step-by-Step Installation Guide

### Step 1: Importing the Kali Image
After downloading the `.7z` or pre-built VirtualBox image from the official Kali website, extract it and double-click the `.vbox` file to import it into VirtualBox.

<img width="1920" height="1080" alt="Screenshot 2026-10-27 140338" src="https://github.com/user-attachments/assets/c80a86f0-ce05-46fa-8639-79c70797c18e" />


### Step 2: Configuring System Settings
Before booting the machine, adjust the Base Memory and Processors to the allocated settings mentioned above.

<img width="1920" height="1080" alt="Screenshot 2026-10-27 140440" src="https://github.com/user-attachments/assets/733bda23-e578-4b80-8b43-b5b38a5a9f6f" />

### Step 3: Network Configuration
Ensuring the network adapter is set to **NAT** so the VM can connect to the internet while remaining secure.

<img width="1920" height="1080" alt="Screenshot 2026-10-27 140615" src="https://github.com/user-attachments/assets/16b0de25-c450-4bbc-b3e7-254335d95436" />

### Step 4: Booting Up & Login
Start the Virtual Machine. Once the boot process is complete, you will be prompted with the login screen.
* **Default Username:** `kali`
* **Default Password:** `kali`

<img width="1920" height="1080" alt="Screenshot 2026-10-27 140909" src="https://github.com/user-attachments/assets/7e5d73c8-2d58-432c-86c6-f09a069689a5" />

### Step 5: Post-Installation (System Update)
The first and most crucial step after setting up any Linux environment is updating the package repositories and upgrading the system. Open the terminal and run:

```bash
sudo apt update && sudo apt full-upgrade -y
