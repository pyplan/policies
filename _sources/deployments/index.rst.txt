============================
Deployments and requirements
============================


Deployment options
==================


Pyplan offers several deployment options:

- **Pyplan Enterprise SaaS**: In order to ensure a strong, secure foundation, Pyplan Cloud shares security responsibilities with an industry-leading cloud infrastructure provider and valued partner such as **Amazon Web Services**. 
  These cloud computing services are used by Pyplan for internal purposes as well as Pyplan clients for their own cloud deployments.

- **On customer cloud**: Pyplan can be deployed in customer clouds (AWS, Azure, GPC, OCI) using the Kubernetes service provided by each cloud provider. 

- **On premise**: Pyplan can be deployed on premise and supports installations in physical or virtualized environments.


----------------------
Pyplan Enterprise SaaS
----------------------

Pyplan Cloud solution offers businesses a world-class analytics and planning platform without the complexities of installing and managing their own deployment.
for more details refer to `Pyplan Enterprise SaaS Overview </index.html#pyplan-enterprise-saas-overview>`__.

-----------------
On customer cloud
-----------------

Pyplan can be deployed on all major cloud providers using the Kubernetes service. The services required depend on each provider.

AWS
---

- VPC
- EKS cluster - K8S API Supported
  
  - v1.22
  
- aws CLI and eksctl CLI
- Enable some EKS Add-ons
  
  - EKS IAM-oidc-provider.
  - EFS-CSI Driver.
  - EKS Autoscaling Driver.
  
- PostgreSQL RDS instance.
- Elastic-cache Redis cluster.
- EKS nodegroups with a specific label.
- Pyplan resource namespace.
- NGINX ingress controller.
- Kubernetes Descheduler.
- Kubernetes Metrics Server
- Fileshare in EFS as persistent volume.
- Bastion host - Linux OS.
- SSL certificate (AWS ACM).

Azure
-----

- AKS cluster - K8S API Supported

  - v1.22
- PostgreSQL Single server.
- 2 AKS nodepool with a specific label.
- Pyplan resource namespace.
- Argo-CD for continuous deployment.
- NGINX ingress controller.
- Kubernetes Descheduler.
- Storage accounts

  - Azure-file premium as persistent volume.
  - A daily backup of the Azure-file created by the Pyplan application, once it is synchronized with Argo-CD.

- Azure VM Bastion machine.
- Internet access to install Pyplan with a helm chart and synchronize the application with Argo-CD.
- A DNS with a valid SSL certificate.



----------
On premise
----------

Pyplan is deployed over MicroK8s, so it requires a Linux distribution which supports snapd.
It can be Debian 10, Ubuntu Server 20.04+, RHEL 7.7+, among others.

Hardware requirements
---------------------

The following table shows the minimum and recommended requirements for 10 simultaneous users.

============================ =========================================== ==========================================
Hardware                      Minimum Configuration                       Recommended Configuration
============================ =========================================== ==========================================
CPU                           3.0GHz Processor (10 logical processors)    3.0GHz Processor (10 logical processors)
RAM                           32 GB (3 GB per user)                       64 GB (6 GB per user)
Disk Space                    100 GB                                      256 GB
File system space allocation  - / → 20GB                                   - / → 30 GB
                              - /var → 30GB                                - /var → 50 GB
                              - /pyplan → 50GB                             - /pyplan → 200 GB
============================ =========================================== ==========================================   


Software requirements
---------------------

- Linux OS
  
  - Debian 10
  - Ubuntu Server 20.04
  - RHEL 7.7 / 8.0 / 8.2 / 8.3
    - Microk8s Service is currently not available for RHEL 8.4.
  - SUSE 15 SP2+

- Server access with 'sudo' permissions to perform the installation of snapd, MicroK8s and other necessary packages.

- Pyplan uses port 443

- Pyplan does not run as root, a user with the following attributes is needed
  - uid: 101010
  - user: pyplan_exec

- An internet connection is required in order to download/install packages and download Pyplan docker images from Docker Hub.

- Once installed, it is necessary to use a web browser (Chrome) to activate Pyplan.

**Special requirements**
RHEL 7.7: It is necessary to enable the following RedHat repositories with
subscription-manager

- "rhel-*-optional-rpms"
- "rhel-*-extras-rpms"

              
Kubernetes Addons
-----------------

Pyplan presents extra configurations which are optional

- Cert-Manager Custom Resource Definition (CRD)

  - An SSL operator that allows anyone to create self-generated certificates for secure connection (HTTPS).
  - A correct DNS configuration is required.
  - The instructions to enable it are detailed in the installation steps.

- K8S Dashboard

  - Official web-based Kubernetes user interface.
  - A correct DNS configuration is required.
  - A valid SSL certificate is mandatory.
  - The instructions to enable it are detailed in the installation steps