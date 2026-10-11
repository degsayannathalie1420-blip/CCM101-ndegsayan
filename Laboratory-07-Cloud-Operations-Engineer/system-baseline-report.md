# System Baseline Report

## 1. Introduction

This report presents the initial resource assessment of the Ubuntu server used in Mission 7. The purpose of the assessment is to understand the host's memory and storage condition before running the web server container.

## 2. Memory Check

The `free -h` command was used to examine the server's memory usage.

* **Total RAM:** 1.9 GiB
* **Used RAM:** 409 MiB
* **Free RAM:** 1.1 GiB
* **Available RAM:** 1.5 GiB
* **Total Swap:** 1.0 GiB
* **Used Swap:** 0 B

The server had 1.5 GiB of available memory when the check was performed. This value provides a useful reference when comparing the host's condition with the memory consumed by the Nginx container.

## 3. Disk Space Check

The `df -h /` command was used to inspect the root filesystem.

* **Filesystem:** `/dev/vda1`
* **Total Capacity:** 19 GiB
* **Used Space:** 5.5 GiB
* **Available Space:** 13 GiB
* **Usage:** 30%

Monitoring disk capacity before a rise in web traffic is important because a nearly full disk can interfere with application logging, temporary files, and other operations needed to keep a service running.

## 4. CPU and Process Observation

The `top` command provides a live view of running processes, CPU activity, and system load. It can help an operator identify resource-intensive processes, although a separate CPU reading was not recorded in this report.

## 5. Screenshots

* `screenshots/memory-check.png`
* `screenshots/disk-check.png`

## 6. Summary

The baseline check recorded 1.9 GiB of RAM and 19 GiB of root filesystem storage. At the time of measurement, 1.5 GiB of memory and 13 GiB of storage were available. These figures serve as a reference for examining the host's condition during the container monitoring activity.
