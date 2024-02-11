# Welcome to openEBS
[![OpenEBS Social Banner](https://github.com/openebs/website/blob/main/website/public/images/png/openebs_github_main_banner_HERO_1.png)](https://www.openebs.io/)

# [openebs.io](https://www.openebs.io/)
OpenEBS is a free openesource Stateful Persistent Data Storage platform for Kubernetes. We are CNCF member project. We are a large global community of K8s Datastorage users.<BR>
<BR>
Our project team was an early pioneering inventor of K8s **Container Native Storage** services. We concieved the vision of a K8s Stateful Persistent data platform that is tightly integrated and embeded natively into the core of K8s.<BR>
<BR>
We have designd and built an innovative ultra High-performance Enterprise grade Block-mode storage Hyper-converged Data Fabric that augments the core storage services of K8s with Stateful Persistence, Enterprise Data mgmt, SSD/NVMe optimized I/O services, Replicated Data volumes, Thin Provisioning, Snapshot and Clones; and many other critical data storage services that don't come in K8s out-of-the-box.<BR>
<BR>

> [!IMPORTANT] > OpenEBS is very popular. Live OpenEBS systems actively report back product metrics every day, to our project Google Anaytics metrics engine (unless disabled by users).
> Here are our key project popularity metrics as of: 01 Feb 2024 <BR>
> * OpenEBS is the #1 deployed Storage Platform for Kubernetes
> * We are the [#1 GitHub Star ranked](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png) K8s Data Storage platform
> * We have +40 Million Volumes deployed globally
> * We have +7 Million Global installations
> * 1 Million OpenEBS K8s Containers are spawned per week
> * 700,000 global users
<BR>

|   |   |
|---|---|
| [![We are builders](https://github.com/openebs/website/blob/main/website/public/images/png/code_icon_200x100.png)](https://github.com/openebs/website/blob/main/website/public/images/png/code_for_success_mantra.png)  | Building a K8s Enterprise Data Storage platform is complex, and areas of the Data & I/O stack could be considerd 'Storage Rocket science'. Our global team comes from many areas of the data storage industry. Companies like... [Microsoft Azure](https://azure.microsoft.com/en-us/), [VMware](https://www.vmware.com/), [DELL/EMC](https://www.dell.com/en-us/shop/scc/sc/storage-products), [Brocade/Broadcom](https://www.broadcom.com/products/fibre-channel-networking), [Hitachi Vantara](https://www.hitachivantara.com/en-us/products/storage-platforms.html), [INTEL](https://www.intel.com/content/www/us/en/products/details/memory-storage.html), [Nvidia/Mellanox](https://developer.nvidia.com/gpudirect-storage), [IBM](https://www.ibm.com/storage), [RedHat](https://www.redhat.com/en/technologies/cloud-computing/openshift) and [DataCore](https://datacore.com). |


Building an Enterprise Data Storage platform is complex, and areas of the Data & I/O stack could be considerd 'Storage Rocket science'. Our global team comes from many areas of the data storage industry. Companies like... [Microsoft Azure](https://azure.microsoft.com/en-us/), [VMware](https://www.vmware.com/), [DELL/EMC](https://www.dell.com/en-us/shop/scc/sc/storage-products), [Brocade/Broadcom](https://www.broadcom.com/products/fibre-channel-networking), [Hitachi Vantara](https://www.hitachivantara.com/en-us/products/storage-platforms.html), [INTEL](https://www.intel.com/content/www/us/en/products/details/memory-storage.html), [Nvidia/Mellanox](https://developer.nvidia.com/gpudirect-storage), [IBM](https://www.ibm.com/storage), [RedHat](https://www.redhat.com/en/technologies/cloud-computing/openshift) and [DataCore](https://datacore.com).<BR>
Our project is grateful for these innovative data storage companies and their amazing storage engineering team contributions. Our orignal founding team continues to guide the project as custodial Maintainers. Major ponsorship is provided via DataCore, Inc (who donates considerable daily Product Dev/Engineering, Product Managment and Program operational rescources to OpenEBS. - Our founding team was acquired by DataCore, Inc). We also have 100's of amazing individuals, contributors and storage engineers who provide brainstorming ideas, feedback, code reviews and high-quality code to the project. - All who are passionate about storage and Data are welcome here.<BR>
<BR>

## Project structure
![](https://github.com/openebs/website/blob/main/website/public/images/png/openebs_github_project-structure.png)

## Deployable Data-Engines
OpenEBS has maintained a steady pace of development & evolution in order to keep in alignment with K8s advancment overall and with the rapid changing pace of technologies, hardware and software innovations in the data stroage industry. The proejct is divided into 2 main deployable Editions :<BR>
| ID  | Edition name  | Data-Engine | Release        |
|-----|---------------|-------------|----------------|
|  1  | Legacy        | [cStor](https://github.com/openebs/cstor-operators)       | [![Releases](https://img.shields.io/github/v/release/openebs/cstor-csi.svg?include_prereleases&style=flat-square)](https://github.com/openebs/cstor-csi/releases)   |
|     |               | [Jiva](https://github.com/openebs/jiva)  | [![Releases](https://img.shields.io/github/v/release/openebs/jiva.svg?include_prereleases&style=flat-square)](https://github.com/openebs/jiva/releases)   |
|     |               | [NFS](https://github.com/openebs/dynamic-nfs-provisioner)  |    |
|  2  | [Standard](https://github.com/openebs/mayastor)     | Mayastor     | [![Releases](https://img.shields.io/github/release/openebs/Mayastor/all.svg?style=flat-square)](https://github.com/openebs/Mayastor/releases)   |
<BR>

## LEGACY
LEGACY consists of Data-Engines that we experimented with early on. These Data-Engines have a number of opensoruce techologies embeded inside them, and are a great intro into the world of simple K8s storage services. LEGACY helped us learn, iterate and develop our core storage K8s strategy, as well as decern how users want & need to interact with K8s storage services. LEGACY also helped to reveal key areas within K8s that are lacking in storage/datastore services,  what areas of K8s we could optimize; and how we can provide the best value into the various K8s storage layers.<BR>
<BR>
There are 3 main Data-Engines in LEGACY:<BR>
| ID  | Data-Eegines      | Embeded tech stack   | Status                           |
|-----|-------------------|----------------------|----------------------------------|
|  1  |  Jiva             | iSCSI                | We plan to sunset LEGACY in 2024 |
|  2  |  cStor            | Open ZFS             | We plan to sunset LEGACY in 2024 |
|  2  |  NFS Provisioner  | NFS userspace server | We plan to sunset LEGACY in 2024 |
<BR>

## STANDARD
**STANDARD** is our Ultra modern Datastore stack that is strongly aligned with the cutting edge direction of storage use-cases in the K8s industry. It is designed to faciliate modern K8s datastore archiectures, key K8s I/O patterns, K8s data access methods, K8s data use-cases and where K8s Datastore applications are heading.
* STANDARD is optimized for NVMe and SSD Flash and integrates ultra modern extreme high performance storage technologies at its core...
    * It uses the High performance [SPDK](https://spdk.io) storage stack - (SPDK is an opensource NVMe project initiated by INTEL)
    * The hyper modern [IO_Uring](https://github.com/axboe/liburing) Linux Kernel Async polling-mode I/O Interface - (fastest kernel I/O mode possible)
    * Native abilties for RDMA and Zero-Copy I/O
    * NVMe-oF TCP Block storage Hyper-converged data fabric
    * Block layer volume replication
    * Logical volumes and Diskpool based data managment
    * a Native high peformance [Blobstore](https://spdk.io/doc/blob.html)
    * Native Block layer Thin provisoning
    * Native Block layer Snapshots and Clones
 <BR>	

There are 2 Data-Engines within the [**STANDARD**](https://github.com/openebs/mayastor) Edition:
| ID  | Data-Eegines       | Type of data services                                  | Status                                                     |
|-----|--------------------|--------------------------------------------------------|------------------------------------------------------------|
|  1  |  **Mayastor**      | Replicated data volumes (a Cluster wide Data fabric)   | Stable, deployable in PROD. Very active development        |
|     | &nbsp;             |                                                        |                                                            |
|  2  |  **Local-PV**      | Non-replicated node local data volumes                 | (Local-PV has multiple variants. See below)                |
|     | &nbsp;             |                                                        |                                                            |
|     |  LVM Local-PV      | for integration with LVM datastor deployments          | Stable, deployable in PROD, undergoing integration         |
|     |  ZFS Local-PV      | for integration with ZFS datastor deployments          | Stable, deployable in PROD, undergoing integration         |
|     |  Local-PV-HostPath | for integration with local node hostpath (/mnt/fs1)    | Stable, deployable in PROD, undergoing integration         |
|     |  Device Local-PV   | for integration with explicit device paths (/dev/sdb)  | Stable, Not deployable in PROD, integration testing        |
|     |  Local-PV-Device   | for integration with NDM managed devices               | Stable, Not deployable in PROD, integration testing        |
|     |  RawFile-Device    | for integration with Soft Luns devices on a filesystem | Stable, deployable in PROD, undergoing integration         |
<BR>

## ROADMAP
Our [2024 Roadmap is here](https://github.com/openebs/openebs/blob/main/ROADMAP.md) It defines a rich set of new featrues that are planned for 2024.<br>
Please review this roadmp and feel free to pass back any feedback on it, as well as recommend and suggest new ideas. We welcome all your feedback.
<br>
<br>

## GitHub Star Chart
OpenEBS is the most successful Stateful Persistent Contianer Native Storage platform in the CNCF landscape. It has allways held the #1 position and continues to as of today.
[![XXXXXXXX](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png)](https://www.openebs.io/)
