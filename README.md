# 🔍 Real-Time Network Traffic Analysis with Snort IDS

> ✅ Task for CodeAlpha Cyber Security Internship  
> 🧑‍💻 Submitted by: **Dawood**

---

## 🎯 Objective

This task demonstrates how to set up a real-time network traffic monitoring and intrusion detection system using **Snort IDS**. It includes simulating attacks (port scanning, DoS), detecting them in real time, and logging the alerts for analysis.

---

## 🛠️ Tools & Technologies Used

| Tool/Service        | Purpose                                      |
|---------------------|----------------------------------------------|
| VirtualBox          | To run a virtual target server               |
| Kali Linux          | Host OS for attack simulation & monitoring   |
| Ubuntu Server 20.04 | Target server (victim machine)               |
| Snort IDS           | Intrusion Detection System                   |
| Nmap                | For performing port scan attacks             |
| Slowloris           | To simulate DoS attacks                      |
| SSH                 | Remote access to the target server           |
| Apache2             | To simulate a running web application        |

---

## ⚙️ Step-by-Step Setup Guide

### 🔸 1. Set Up Virtual Environment
- Install **VirtualBox** on Kali Linux.  
  ➤ [Official Guide](https://www.kali.org/docs/virtualization/install-virtualbox-host/)

- Download the **Ubuntu Server ISO**:  
  ➤ [Ubuntu Server Download](https://ubuntu.com/download/server)

- Create a new virtual machine in VirtualBox:
  - Click "New", name the VM, and select the ISO
  - Follow the installation steps

---

### 🔸 2. Prepare the Ubuntu Server (Target)
```bash
sudo apt install openssh-server    # (Optional)
sudo apt install snort
