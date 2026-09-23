# MinIO Deployment

## Overview

MinIO was deployed as an S3-compatible object storage service using Docker. The container exposed ports 9000 and 9001, with port 9001 used for the MinIO web console.

## Deployment Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
```

## Ports

| Port | Function      |
| ---- | ------------- |
| 9000 | MinIO API     |
| 9001 | MinIO Console |

## Environment Variables

The `MINIO_ROOT_USER` variable defines the administrator username used when accessing the MinIO service.

The `MINIO_ROOT_PASSWORD` variable defines the administrator password.

These variables provide the initial credentials for the MinIO administrator account.

## Bucket

The bucket created for the laboratory was:

`client-photos`

A sample object was uploaded to the bucket through the MinIO Console.

## Container Verification

The following command was used to check whether the MinIO container was running:

```bash
docker ps
```

The `minio-server` container was displayed as running before continuing to the web console.
