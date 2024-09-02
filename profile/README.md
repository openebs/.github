# Welcome to [OpenEBS](https://github.com/openebs/openebs)
<!--- [![OpenEBS Social Banner](https://github.com/openebs/website/blob/main/website/public/images/png/openebs_github_main_banner_HERO_1.png)](https://www.openebs.io/) -->
[![OpenEBS Social Banner](https://github.com/openEBS/community/blob/develop/images/forest-road-game-pixel-art_HERO_banner.png)](https://www.openebs.io/)

| Quick links  |  [```CNCF openebs website ```](https://www.openebs.io/)  |  [``` CNCF Product docs ```](https://www.openebs.io/docs)  | [``` Main Parent repo ```](https://github.com/openebs/openebs) |  [``` Community Cafe ```](https://github.com/openebs/community?tab=readme-ov-file#community-repo-cafe) |  [``` Community Meeting ```](https://github.com/openebs#monthly-community-meetings) |
| :---:        |              :---:             |            :---:             |            :---:             |            :---:             | :---:        |

---
## Project Purpose

OpenEBS is an open-source storage service for Kubernetes applications. OpenEBS manages the block storage and file systems based on the block storage for containers running in Kubernetes. Use OpenEBS for creating fast and resilient storage; with options for single-node, and replicated multi-node storage.

OpenEBS is a Stateful Persistent block-mode Data Storage platform with a native vSAN fabric; for Kubernetes. We are a CNCF member project. We are the largest global community of K8s storage users.<BR>
<BR>
Our project team was an early pioneering inventor of K8s **Container Native Storage** services (we invented the term). We conceived the vision of a Stateful Persistent data platform for K8s that is tightly integrated and natively embedded into the core of K8s.<BR>
<BR>
We built an innovative High-performance Enterprise grade Block-mode Hyper-converged Storage vSAN Fabric that augments the storage services of K8s with Stateful Persistence, Enterprise Data mgmt, SSD/NVMe optimized I/O services, Replicated Data volumes, Thin Provisioning, Snapshot, Clones; and many other Mission critical data storage services that ```don't come``` in K8s out-of-the-box.<BR>
<BR>

> **OpenEBS is very popular :** <BR>
> Live OpenEBS systems actively report back product telemetry each day, to our Global Analytics system (unless disabled by the user).<BR>
> Below are our project popularity & penetration metrics as of: <kbd>01 May 2024</kbd> <BR>
>
> :rocket: &nbsp; OpenEBS is the **#1 deployed** Storage ```Platform``` for Kubernetes <BR>
> :star: &nbsp; We are the [#1 GitHub Star ranked](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png) K8s Data Storage platform <BR>
> :floppy_disk: &nbsp; We have **+49 Million** <kbd>Volumes</kbd> deployed globally <BR>
> :tv: &nbsp; We have **+9 Million** Global Live <kbd>Nodes</kbd> <BR>
> :zap: &nbsp; **1 Million** OpenEBS K8s Containers are ```spawned per week``` <BR>
> :sunglasses: &nbsp; **1.7 Million** ```User Installations ``` <BR>

| [<img src="https://github.com/openebs/community/blob/develop/images/code_for_success_mantra_small.png" align="center" width="450px"/>](https://github.com/openebs/community) | Our global team comes from many areas of the data storage industry. Companies like... [Microsoft Azure](https://azure.microsoft.com/en-us/), [VMware](https://www.vmware.com/), [DELL/EMC](https://www.dell.com/en-us/shop/scc/sc/storage-products), [Brocade/Broadcom](https://www.broadcom.com/products/fibre-channel-networking), [Hitachi Vantara](https://www.hitachivantara.com/en-us/products/storage-platforms.html), [INTEL](https://www.intel.com/content/www/us/en/products/details/memory-storage.html), [Nvidia/Mellanox](https://developer.nvidia.com/gpudirect-storage), [IBM](https://www.ibm.com/storage), [RedHat](https://www.redhat.com/en/technologies/cloud-computing/openshift) and [DataCore](https://datacore.com).  |
| :---  | :--- |
<BR>

[![Project Structure](https://github.com/openebs/community/blob/develop/images/island-beach_pixel-art_STORAGE-ENGINES_banner.png)](https://github.com/openebs/community/)

## Why OpenEBS?
OpenEBS provides enterprise-grade data management for Kubernetes clusters, with five different storage engines (four single-node and one replicated) that meet a range of use cases for Kubernetes users. The five engines are summarized in the table below:
<BR>
> [!IMPORTANT]
> The openEBS platform, provides 2 types of K8s Storage Services. ```Replicated PV``` and ```Local PV```.
<BR>

| Engine | [Local PV HostPath](https://github.com/openebs/dynamic-localpv-provisioner) | [Local PV ZFS](https://github.com/openebs/zfs-localpv) | [Local PV LVM](https://github.com/openebs/lvm-localpv)  | [Local PV Rawfile](https://github.com/openebs/rawfile-localpv) | [Replicated PV Mayastor](https://github.com/openebs/mayastor) |
| :---:  | :---              | :---         | :---         | :---:            | :---:                  | 
| Type   | Single-node       | Single-node  | Single-node  |  Single-node     | Multi-node             |
| What is it for?   | Replacement for in-Tree Kubernetes CSI HostPath       | Storage engine for ZFS managed backend storage  | Storage engine for LVM2 managed backend storage  |  Experimental engine for using an extent file as block storage     | General purpose replicated enterprise storage           |
| Designed for | Developers or DevOps | ZFS users and production deployments | LVM2 users and production deployments | Developers | Enterprises and production deployments |
| Features | Everything in Kubernetes HostPath, plus: - Dynamic provisioning, Zero configuration, No CSI driver | Provision ZFS datasets, Provision ZFS volumes, Dynamic provisioning, ZFS resilience, ZFS RAID protection, CSI driver | Provision LVM2 volumes, Dynamic provisioning, LVM2 RAID protection, CSI driver | Provision file system from local files as persistent volumes, CSI driver | Replicated storage NVMe / RDMA, Snapshots, Clones, High availability, CSI driver|
| Status | Stable, deployable in PROD  | Stable, deployable in PROD  | Stable, deployable in PROD  | Beta, undergoing evaluation & integration | Stable, deployable in PROD  | 
| Current Version | [![Releases](https://img.shields.io/github/release/openebs/dynamic-localpv-provisioner/all.svg?style=flat-square)]() | ![Releases](https://img.shields.io/github/release/openebs/zfs-localpv/all.svg?style=flat-square) | [![Releases](https://img.shields.io/github/release/openebs/lvm-localpv/all.svg?style=flat-square)]() | ```release: v0.70``` | [![Releases](https://img.shields.io/github/release/openebs/Mayastor/all.svg?style=flat-square)]() | 

<BR>

We are an Ultra modern Data storage platform stack that is strongly aligned with the cutting-edge direction of storage use cases in the K8s industry. openEBS is designed to facilitate modern K8s datastore architectures, key K8s I/O patterns, K8s data access methods, K8s data use-cases and where K8s Datastore applications are heading.
<BR>	

OpenEBS is optimized for NVMe and SSD Flash storage media and integrates ultra-modern cutting-edge high-performance storage technologies at its core.</summary>

>
> :ballot_box_with_check: &nbsp; It uses the High performance [SPDK](https://spdk.io) storage stack - (SPDK is an open-source NVMe project initiated by INTEL) <BR>
> :ballot_box_with_check: &nbsp; The hyper-modern [IO_Uring](https://github.com/axboe/liburing) Linux Kernel Async polling-mode I/O Interface - (fastest kernel I/O mode possible) <BR>
> :ballot_box_with_check: &nbsp; Native abilities for RDMA and Zero-Copy I/O <BR>
> :ballot_box_with_check: &nbsp; NVMe-oF TCP Block storage Hyper-converged data fabric <BR>
> :ballot_box_with_check: &nbsp; Block layer volume replication <BR>
> :ballot_box_with_check: &nbsp; Logical volumes and Diskpool based data management <BR>
> :ballot_box_with_check: &nbsp; a Native high performance [Blobstore](https://spdk.io/doc/blob.html) <BR>
> :ballot_box_with_check: &nbsp; Native Block layer Thin provisioning <BR>
> :ballot_box_with_check: &nbsp; Native Block layer Snapshots and Clones <BR>

</details>
<BR>

---

> [!WARNING]
> ### ```LEGACY Edition```
> Legacy has been <KBD> archived </KBD> and migrated out of the main openEBS parent repo.
```Erlang
LEGACY consists of Data-Engines that we experimented with early on. These Data-Engines have a number of open-source
technologies embedded inside them, and are a great intro into the world of simple K8s storage services. LEGACY helped
us learn, iterate, and develop our core storage K8s strategy, as well as discern how users want & need to interact with
K8s storage services. LEGACY also helped to reveal key areas within K8s that are lacking in storage/datastore services,
what areas of K8s we could optimize; and how we can provide the best value into the various K8s storage layers.
```

<BR>

There are multiple Storage Engines within LEGACY:<BR>
| ID  | Data-Engines      | Embedded tech stack   | Status        | Action date  |
|:---:|:---               | :----                |:---           | :---         |
|  |  | &nbsp;  |  |  |
|  1  |  Jiva             | iSCSI                | ```deprecated``` & has been ```Migrated``` to [OpenEBS Archive org](https://github.com/openebs-archive/jiva) | 29 Apr, 2024 |
|  2  |  cStor            | Open ZFS             | ```deprecated``` & has been ```Migrated``` to [OpenEBS Archive org](https://github.com/openebs-archive/cstor-csi) | 29 Apr, 2024 |
|  3  |  NFS Provisioner  | NFS userspace server | ```deprecated``` & has been ```Migrated``` to [OpenEBS Archive org](https://github.com/openebs-archive/dynamic-nfs-provisioner) | 29 Apr, 2024 |
|  4  |  Device LocalPV     | Node Local storage   | ```deprecated``` & has been ```Migrated``` to [OpenEBS Archive org](https://github.com/openebs-archive/device-localpv) | 29 Apr, 2024 |
|  5  |  LocalPV Device     | Node Local storage   | ```deprecated``` & has been ```Migrated``` to [OpenEBS Archive org](https://github.com/openebs-archive/) | 29 Apr, 2024 |
|  6  |  NDM              | Node Local storage   | ```deprecated``` & has been ```Migrated``` to [OpenEBS Archive org](https://github.com/openebs-archive/node-disk-manager) | 29 Apr, 2024 |
|  7  |  +43 other repos & projects<BR>(Total Repos migrated: 49)| 66% of Project's repos have been Archvied  | Please see the [OpenEBS Archive org](https://github.com/openebs-archive/) | 29 Apr, 2024 |
<BR>

---

## :earth_americas: ROADMAP
Our [2024 Roadmap is here](https://github.com/openebs/openebs/blob/main/ROADMAP.md) It defines a rich set of new features that are planned for 2024.<br>
Please review this roadmap and feel free to pass back any feedback on it, as well as recommend and suggest new ideas. We welcome all of your feedback.
<br>
<br>

## :star: GitHub Star Chart
OpenEBS is the most successful Stateful Persistent Container Native Storage platform in the CNCF landscape. It has always held the #1 position and continues to as of today.

[![XXXXXXXX](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png)](https://www.openebs.io/)

> [!IMPORTANT]
> Our original founding team guides the project as Maintainers. Major sponsorship is provided by [DataCore](https://datacore.com), which donates a large team of dedicated Product Dev/Engineers, Product Mgmt, and operational resources. OpenEBS has hundreds of amazing contributors and storage engineers who provide ideas, feedback, and high-quality code to the project. - Everyone is welcome.

## Community Resources
We centralize all our community documentation in the [Community](https://github.com/openebs/community) repo. All sub-projects within the organization follow the same umbrella policies, except where stated in the sub-project readme.

## Monthly community meeting
OpenEBS holds a monthly community meeting via Zoom on the last Thursday of the month, at 7 am Pacific time.
<br>
The next meeting is on: `Thursday 26 September, at 14:00 UTC`
<br>
Meeting Link: https://us05web.zoom.us/j/87535654586?pwd=CigbXigJPn38USc6Vuzt7qSVFoO79X.1
<br>
Starting in August 2024, the meetings will be recorded and posted on YouTube.

## Other Resources
Maintainers meet weekly and minute their meetings. A public record of the meetings is here.
See [Vision](https://github.com/openebs/community/blob/develop/VISION.md) for more detail on what we do, [Governance](https://github.com/openebs/community/blob/develop/GOVERNANCE.md) for how we do it, and [Contributing](https://github.com/openebs/community/blob/develop/CONTRIBUTING.md) for how to get involved

## New Contributors and Maintainers
We are actively looking for new contributors and maintainers. Want to get involved, but not sure how? Please email the OpenEBS maintainers at openebs.team@gmail.com

