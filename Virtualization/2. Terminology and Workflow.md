# Key Terminologies

### 1. Host Machine

- The physical computer or server where virtualization software is installed.

#### Features:
- Provides CPU, RAM, storage, and network
- Runs multiple virtual machines
- Controls hardware resources

#### Example:
A physical Dell server running VMware ESXi.

### 2. Guest Machine
- A virtual machine running inside the host machine.

#### Features:
- Has its own OS and applications
- Uses virtual resources from host
- Works independently from other VMs

Example:
Ubuntu VM running inside VirtualBox.

### 3. Hypervisor
- Software that creates, manages, and controls virtual machines.

#### Functions:
- Allocates hardware resources
- Starts and stops VMs
- Maintains isolation between VMs

#### Types:
- Type 1 hypervisor ( Bare Metal Hypervisor ) runs directly on physical hardware without any operating system.
- Used for Production purpose, more secure and faster.
            
                 Architecture:
            
            +----------------------+
            | Virtual Machines     |
            +----------------------+
            | Type 1 Hypervisor    |
            +----------------------+
            | Physical Hardware    |
            +----------------------+
  - Examples: VMware ESXi, Microsoft Hyper-V 
- Type 2 hypervisor ( Hosted Hypervisor ) runs on top of operating system
- Used for testing and leaning purposes but its slower.

                Architecture:
            
            +----------------------+
            | Virtual Machines     |
            +----------------------+
            | Type 2 Hypervisor    |
            +----------------------+
            | Host Operating System|
            +----------------------+
            | Physical Hardware    |
            +----------------------+

  - Examples: Oracle VirtualBox, VMware Workstation

### 4. VM provisioning 
-   Provisioning is the automated process of creating, configuring, and deploying virtual machines (VMs) by allocating CPU, memory, storage, and network resources to meet specific user needs. I

### 5. Virtual Machine (VM)
- A software-based computer that behaves like a physical computer.

VM Includes:
- Virtual CPU
- Virtual RAM
- Virtual Disk
- Virtual Network Adapter
- Operating System

### 6. Snapshot
- A saved state or "at a point of time" of a virtual machine.(not backup)

Uses:
- Restore VM during failure
- Testing and rollback
- Safe software updates

Advantages:
- Quick recovery
- Saves VM state instantly
- Helps in troubleshooting

Example:
Taking snapshot before installing software updates.


## Simple Workflow:

1. Physical Computer
- The real machine containing CPU, RAM, and storage.
---
       
2. Hypervisor
- Software installed to create and manage virtual machines.
---
3. Virtual Machine (VM)
- A virtual computer created by the hypervisor.
---
4. Operating System
- OS like Ubuntu or Windows installed inside VM.
---

5. Applications
- Software and programs installed inside the VM.
---

6. VM Running
- VM works like a normal computer independently.
