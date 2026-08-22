# System Information

This document contains the basic system information collected from the Ubuntu 24.04 Linux environment provided through the KillerCoda Playground.

## Linux Distribution

**Ubuntu 24.04**

The system is running Ubuntu 24.04, a Linux distribution commonly used for servers, development environments, and cloud infrastructure. In this activity, Ubuntu provides the operating environment where I performed the Linux commands and created my files.

## Kernel Version

**6.8.0-136-generic**

The kernel version is 6.8.0-136-generic. The Linux kernel is the main part of the operating system that manages the communication between the software and the computer's hardware resources.

## CPU Information

**Intel Xeon E312xx (Sandy Bridge, IBRS update)**

The environment is using an Intel Xeon E312xx processor based on the Sandy Bridge architecture. Since KillerCoda provides a cloud-based environment, this represents the CPU resources available to the virtual machine rather than a physical computer that I personally own.

## Total Memory

```text
              total        used        free      shared  buff/cache   available
Mem:           1.9Gi       447Mi       797Mi       1.1Mi       827Mi       1.4G
```

The system has **1.9 GiB of total memory**. At the time the information was collected, around **447 MiB was being used**, while **797 MiB was free**. The system also had **827 MiB allocated to buffers and cache**. The available memory was approximately **1.4 GiB**, which means the environment still had a reasonable amount of memory available for additional processes.

## Available Disk Space

```text
/dev/vda1        19G  5.4G   13G  30% /
/dev/vda16      881M  117M   703M  15% /boot
/dev/vda15      105M  6.2M    99M   6% /boot/efi
```

The main filesystem has **19 GB of total storage**, with approximately **5.4 GB already used** and **13 GB available**. Around **30% of the main filesystem is being used**.

The `/boot` partition has **881 MB of total space**, with **117 MB used** and approximately **703 MB available**. It is currently using about **15%** of its storage.

The `/boot/efi` partition has **105 MB of total space**, with only **6.2 MB used** and about **99 MB available**. This means approximately **6%** of that partition is being used.

## Summary

The KillerCoda environment provides a small but usable Ubuntu Linux system. It has 1.9 GiB of memory and a 19 GB main filesystem, with enough available resources to complete the activities in this laboratory. Checking these details helped me understand the resources available in a cloud-based Linux environment.
