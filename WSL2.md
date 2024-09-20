# Windows Subsystem for Linux 2 (WSL2) - Everything You Need to Know

## Table of Contents
- [What is WSL2?](#what-is-wsl2)
- [Benefits of WSL2](#benefits-of-wsl2)
- [Key Features](#key-features)
- [System Requirements](#system-requirements)
- [Installation](#installation)
- [Do's and Best Practices](#dos-and-best-practices)
- [Troubleshooting and Common Issues](#troubleshooting-and-common-issues)

## What is WSL2?
Windows Subsystem for Linux 2 (WSL2) is a feature in Windows that allows users to run a Linux kernel on their Windows system. It provides better performance and full compatibility with Linux software, compared to WSL1.

WSL2 uses a lightweight virtual machine (VM) and offers improved file system performance. It is a great tool for developers who want the best of both Windows and Linux operating systems.

---

## Benefits of WSL2
- **Full Linux Kernel**: WSL2 includes a full Linux kernel built by Microsoft, allowing for system calls, compatibility with Linux applications, and better overall performance.
- **Improved File I/O Performance**: WSL2 offers faster file system performance compared to WSL1, especially when dealing with heavy workloads.
- **Better Docker Integration**: Since WSL2 uses a VM, Docker can run natively without requiring Docker Desktop, providing a smoother developer experience.
- **Low Resource Usage**: Although WSL2 uses a VM, it is lightweight compared to traditional virtual machines and uses fewer system resources (RAM, CPU).
- **Seamless Windows Integration**: You can access Windows files from the Linux environment, and vice versa. This allows you to work fluidly between both operating systems.

---

## Key Features
- **Native Linux Kernel**: Allows for greater compatibility with Linux tools and services.
- **Virtualized Environment**: Runs a true Linux kernel using lightweight virtualization.
- **File System Support**: Provides a fast and efficient file system for developers.
- **Memory Management**: Dynamically uses system resources, scaling RAM usage up and down based on the workload.

---

## System Requirements
- **Windows 10 Version 1903** or higher (Build 18362 or higher)
- **Windows 11** fully supports WSL2
- **Windows Hyper-V** and **Virtual Machine Platform** must be enabled.

---

## Installation

1. **Enable WSL and Virtual Machine Platform**:
   ```bash
   dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
   dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
