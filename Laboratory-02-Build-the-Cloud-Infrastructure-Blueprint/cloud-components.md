# Understanding Cloud Infrastructure Components

## Compute

Compute resources are responsible for executing programs and processing requests. The processor performs calculations, while memory temporarily holds information required by running applications.

### Why Compute Matters

Applications cannot operate without processing resources. Cloud platforms allow organizations to use virtual computing resources without needing to own every physical server.

### Laboratory Example

The investigated KillerCoda environment has one CPU core and approximately 1.9 GiB of memory.

---

## Storage

Storage provides a location for system files, applications, documents, and other information that must be retained.

### Why Storage Matters

Cloud systems need reliable storage because important data should remain available after an application finishes running. Storage also supports backups and long-term data retention.

### Laboratory Example

The main storage volume is /dev/vda1. It uses the ext4 filesystem and provides a total capacity of 19 GB.

---

## Networking

Networking connects cloud resources and allows information to travel between systems.

### Why Networking Matters

Users need network access to reach online applications and services. Networking also allows cloud servers, databases, and other resources to communicate.

### Laboratory Example

The primary interface is enp1s0, and the recorded IPv4 address is 172.30.1.2/24.

---

## Operating System

The operating system provides the software environment needed to manage a server.

### Why the Operating System Matters

It manages processes, files, users, memory, and network operations. It also provides the tools used by administrators to monitor and configure infrastructure.

### Laboratory Example

The server operates using Ubuntu 24.04.4 LTS and Linux kernel 6.8.0-138-generic.

---

## Working as One Infrastructure

A cloud environment functions because its resources work together. The operating system coordinates the resources, compute performs processing, storage keeps information, and networking provides communication between the system and external users or services.
