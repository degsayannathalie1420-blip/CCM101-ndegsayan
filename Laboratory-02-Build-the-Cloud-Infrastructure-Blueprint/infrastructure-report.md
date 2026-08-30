# Linux Infrastructure Report

## System Information

| Item             | Information Collected                         |
| ---------------- | --------------------------------------------- |
| Operating System | Ubuntu 24.04.4 LTS                            |
| Linux Kernel     | 6.8.0-138-generic                             |
| Processor Model  | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| Number of Cores  | 1                                             |
| Total Memory     | 1.9 GiB                                       |
| System Hostname  | ubuntu                                        |

### Findings

The environment used for this laboratory is a virtual Linux system running Ubuntu 24.04.4 LTS. It is equipped with a single CPU core and approximately 1.9 GiB of memory. The Linux kernel coordinates the available hardware resources and allows the operating system and applications to function correctly.

## Network Information

| Item                 | Information Collected |
| -------------------- | --------------------- |
| Active Interface     | enp1s0                |
| Interface Status     | UP                    |
| Main IPv4 Address    | 172.30.1.2/24         |
| Loopback Address     | 127.0.0.1/8           |
| Additional Interface | docker0               |
| Docker Network       | 172.17.0.1/16         |

### Findings

The main connection of the virtual machine is provided through the enp1s0 interface. Since its status is UP, the interface is active and available for network communication. The loopback address is used for internal communication, while docker0 is related to the networking environment used by containers.

## Storage Information

| Filesystem | Format | Size | Used | Available | Usage | Mount Point |
| ---------- | ------ | ---: | ---: | --------: | ----: | ----------- |
| /dev/vda1  | ext4   |  19G | 5.4G |       13G |   30% | /           |
| /dev/vda16 | ext4   | 881M | 117M |      703M |   15% | /boot       |
| /dev/vda15 | vfat   | 105M | 6.2M |       99M |    6% | /boot/efi   |

### Findings

The root filesystem is stored on /dev/vda1, making it the main storage area of the Linux environment. The device uses the ext4 format and still has approximately 13 GB available. Separate partitions are maintained for boot files and EFI system information.

## Infrastructure Summary

The environment contains the essential elements of a cloud server. Processing tasks depend on the CPU and memory, files are maintained through storage devices, and communication is supported by network interfaces. Ubuntu Linux brings these resources together into one working system.
