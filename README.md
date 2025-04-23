# VProfile-DevOps-Project-Setup-Manual-&-Automated-

This repository contains the VProfile DevOps project setup using Vagrant for multi-VM environments. It supports both manual provisioning and automated provisioning tailored for Windows, Mac, and Intel systems.

<h2>🚀 Project Overview</h2>
This project creates multiple virtual machines (VMs) using Vagrant for a complete application stack consisting of:

--> Frontend (nginx)

--> Backend (Tomcat)

--> Database (MySQL)

--> Caching (Memcached)

--> Messaging (RabbitMQ)

You can choose between two modes:

<h2>🔧 Manual Provisioning </h2>
Folder: Manual_provisioning_WinMacIntel/

<h3>📌 Steps:</h3>
1. Follow the PDF guide <h4>VprofileProjectSetupWindowsAndMacIntel.pdf</h4> for detailed step-by-step instructions.

2. Manually SSH into each VM and install dependencies.

3. Great for beginners who want to understand the inner workings of DevOps setup.

<h2>⚙️ Automated Provisioning</h2>
Folder: Automated_provisioning_WinMacIntel/

<h3>📌 Steps:</h3>
1. Navigate to the directory:

```
cd Automated_provisioning_WinMacIntel
```
2. Run:
```
vagrant up
```

✅ This will:

Launch all required VMs.

Automatically configure each service (nginx, mysql, tomcat, rabbitmq, memcached).

Use shell scripts to install and configure services.

Download application files and copy necessary configurations.

This approach is ideal for quickly spinning up the full stack with minimal manual effort.

<h2>🧪 Requirements </h2>
Vagrant 2.x

VirtualBox

Verified on Windows and Intel machines.

<h2>📎 Tips </h2>
Use vagrant ssh <vm-name>(example: web01, db01) to access any specific VM.

To halt(stop) VMs: vagrant halt

To remove(delete) all VMs: vagrant destroy -force

<h2>🙌 Author</h2>
Maintained by Fuzail Ahamad
