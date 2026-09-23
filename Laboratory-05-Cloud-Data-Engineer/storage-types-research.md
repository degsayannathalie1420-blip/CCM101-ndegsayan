# Storage Types Research

## Cloud Storage Comparison

| Storage Type   | Description                                                                                                             | Primary Use Case                                                            | Cloud Provider Example |
| -------------- | ----------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- | ---------------------- |
| Block Storage  | Data is divided into blocks and presented to a system as storage that can be attached to a computer or virtual machine. | Databases, virtual machines, and applications requiring disk storage.       | AWS EBS                |
| File Storage   | Data is organized into files and folders through a shared file system.                                                  | Shared folders, documents, and applications that require file-based access. | AWS EFS                |
| Object Storage | Data is stored as individual objects together with metadata and an identifier.                                          | Photos, videos, backups, documents, and other unstructured data.            | Amazon S3              |

## Why Object Storage Fits the Client's Requirement

Object storage is appropriate for a photo-sharing application because images are unstructured files that can be stored as separate objects. It can organize large numbers of files in buckets while allowing applications to access the objects when they are needed.
