# Storage@Google Cloud
This is a high-level overview of important storage infrastructure services in Google Cloud.
## STORE
This section details the different storage options available within Google Cloud, categorized by their underlying technology:
### Block
Provides block-level storage, similar to hard drives
#### [PD (Persistent Disk)](https://cloud.google.com/compute/docs/disks?_gl=1*1khelqm*_up*MQ..&gclid=CjwKCAjw5qC2BhB8EiwAvqa41oQQQxMNeSkD3pa0T1Ylg0lI4yRraoDUEYsaFMZKrAitYotvtOEKKhoCcy8QAvD_BwE&gclsrc=aw.ds#pdspecs)
Dedicated hard-disk drives (HDD) and solid-state drives (SSD) for enterprise and database applications deployed to Compute Engine VMs and Google Kubernetes Engine (GKE) clusters.
#### [Hyperdisk](https://cloud.google.com/compute/docs/disks?_gl=1*1khelqm*_up*MQ..&gclid=CjwKCAjw5qC2BhB8EiwAvqa41oQQQxMNeSkD3pa0T1Ylg0lI4yRraoDUEYsaFMZKrAitYotvtOEKKhoCcy8QAvD_BwE&gclsrc=aw.ds#hyperdisks)
Hyperdisk is the newest generation of network block storage service in Google Cloud.
#### [Local SSD](https://cloud.google.com/compute/docs/disks/local-ssd)
Ephemeral, locally attached block storage for high-performance applications.
### File
#### [Filestore](https://cloud.google.com/filestore/docs/overview)
NFSv3 file servers for Compute Engine VMs and Google Kubernetes Engine clusters.
#### [NetApp Volumes](https://cloud.google.com/netapp/volumes/docs/discover/overview)
File-based storage using NFSv3, NFSv4.1, or SMB.
#### [Parallelstore (Private Preview)](https://cloud.google.com/parallelstore?hl=en)
High performance, managed parallel file service
### Object
#### [Cloud Storage](https://cloud.google.com/storage/docs/introduction)
Cloud Storage is a managed service for storing unstructured data. Store any amount of data and retrieve it as often as you like.
## MIGRATE
### [ONLINE: STS(Storage Transfer Service)](https://cloud.google.com/storage-transfer/docs/overview)
Storage Transfer Service automates the transfer of data to, from, and between object and file storage systems.
### [OFFLINE:TA(Transfer Appliance)](https://cloud.google.com/transfer-appliance/docs/4.0/order-appliance) 
High-capacity storage device that enables you to transfer and securely ship your data to a Google upload facility, where we upload your data to Cloud Storage. 
### Other Tools:
[`gcloud storage cp`](https://cloud.google.com/sdk/gcloud/reference/storage/cp)
## PROTECT
### Primitives
### [Backup & DR](https://cloud.google.com/backup-disaster-recovery/docs/concepts/backup-dr)
Managed backup and disaster recovery (DR) service for centralized, application-consistent data protection. Protect workloads by backing them up to Google Cloud.
### [Backup for GKE](https://cloud.google.com/kubernetes-engine/docs/add-on/backup-for-gke/concepts/backup-for-gke)
Backup for GKE is a service for backing up and restoring workloads in GKE clusters.
## References
[Design an optimal storage strategy for your cloud workload](https://cloud.google.com/architecture/storage-advisor#file-storage)  
[Migrate to Google Cloud: Transfer your large datasets](https://cloud.google.com/architecture/migration-to-gcp-assessing-and-discovering-your-workloads)
