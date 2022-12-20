Frequently asked questions
==========================

What are the infrastructure certifications ?
--------------------------------------------

https://aws.amazon.com/compliance/iso-certified/ 


Environmental conditions are monitored and regulated ?
------------------------------------------------------

https://aws.amazon.com/compliance/data-center/environmental-layer/ 


Are system and security patches applied to workstations on a regular basis?
---------------------------------------------------------------------------
Yes, all workstations have automatic system updates. Workstations are regularly monitored.


Do your developers undergo training to ensure knowledge of security standards and industry best practices ?
-----------------------------------------------------------------------------------------------------------
Yes, we conduct annual workshops where we review security issues at both the application and network level.

Do you have a policy for managing access to the program source code?
--------------------------------------------------------------------
Access to the source code is limited to developers and code administrators only. 
Each developer has access only to the repository he/she is working on.
Source code is managed in private GIT repositories with appropriate security restrictions.


Do you have procedures in place to ensure that only authorized individuals have access to the program source code?
------------------------------------------------------------------------------------------------------------------
Only the source code administrator has the capability to add/remove permissions on repositories.
In the "off-boarding" process, access to the repositories is removed.


Are all employees required to undergo incident and breach response training
---------------------------------------------------------------------------
As part of the on-boarding process, a cybersecurity officer meets with the new employee and they review the content related to security and data processing.


What are your network security policies for your office locations?
------------------------------------------------------------------
In order to ensure a strong, secure foundation, Pyplan Cloud shares security responsibilities with an industry leading cloud infrastructure vendor and valued partner.
All data is stored using AWS services, in private networks that can only be accessed through the application.

The security policies in our offices are as follows:

- Access to the local network is through mac address registration. 
- The local network is segmented in 3 sub-networks (not accessible to each other):
  
  - main network
  - secondary network
  - guest network
- Access administration is performed by qualified personnel, with clear and defined responsibilities.



Do you require all workstations to have antivirus/anti-malware software installed?
----------------------------------------------------------------------------------

We use McAfee with automatic updates 


Do you have an Intrusion Detection System/Intrusion Prevention System in place?
-------------------------------------------------------------------------------

We use Amazon GuardDuty for this purpose


Do you have a mobile device policy?
-----------------------------------

In order to ensure a strong, secure foundation, Pyplan Cloud shares security responsibilities with an industry leading cloud infrastructure vendor and valued partner.
All data is stored using AWS services, in private networks that can only be accessed through the application.
Since the data is stored only using AWS services, the mobile phone usage policies are reduced to the following:

- prior to initial use on the network or related infrastructure, all personally owned mobile devices must be registered with IT.
- utilize a device lock with authentication, such as a fingerprint or strong password, on each participating device. Refer to the  password policy for additional information.
- it is essential that mobile users not use unencrypted connections to WiFi access points, and even encrypted public WiFi access should only be used if absolutely necessary.
- employees agree to never disclose their passwords to anyone, particularly to family members, if business work is conducted from home.
- exercise reasonable physical security measures. It is the end users responsibility to keep their equipment safe and secure.
- a device's firmware/operating system must be up-to-date in order to prevent vulnerabilities and make the device more stable. The patching and updating processes are the responsibility of the owner.
- any non-corporate computers used to synchronize with the  equipment will have installed anti-virus and anti-malware software deemed necessary by IT Department. Anti-virus signature files must be up to date on any additional client machines – such as a home PC – on which this media will be accessed.


Do you require employees to use VPNs when accessing the network and information systems from outside of the office (i.e., remotely)?
------------------------------------------------------------------------------------------------------------------------------------

Infrastructure administrator users need to use VPN + MFA + IP Filtering to access the network where the infrastructure is located (AWS).
Application end users only access via web browser using secure protocols (TLS).

Do you have hardening controls in place?
----------------------------------------

Controls performed for hardening are:

- Default passwords: The passwords generated by default for all services/applications must be changed following the password policy.
- Hardcoded passwords and other credentials stored in plain text.
- Lack, or deficiency, of privileged access controls.
- Unencrypted, or inadequately encrypted, network traffic or data at rest.

Data segregation
----------------

Pyplan is deployed on Kubernetes. When a user logs into the Pyplan, a dedicated user pod is created and that pod only has access to the disk drive assigned to the user's company.


Do you have a change management process
---------------------------------------

Change management is the process established to understand and minimize risks while making changes. The main objective is to ensure that changes are executed with as much control and predictability as possible, while minimally affecting the service being changed.

 
The change process occurs in three steps:

1. Request
2. Execution
3. Preparation
4. Implementation

 
**Request**: 
The beginning of the cycle of change of an application is initiated with a formal request for service through a form by the customer areas. From this request, the Systems area performs an analysis and, if necessary, initiates the change of the application.

 

**Execution**:
The execution of the change may involve several items such as systems, infrastructure, processes, etc., involving the following steps:

* Development
* Testing
* Homologation

 

**Preparation**:
After the approval of the change by the requester, the process of implementing the change begins. This process includes the following activities:

* Plan the implementation of the change
* Schedule the change (according to the change window of each application)
* Notify those involved (areas involved, customers, etc.)
  
To start the implementation process you must:

* Fill out the document that contains the main information for planning the execution of the change
* Fill out the spreadsheet that contains the steps to be carried out
* Request authorization from the application owner using the form
* If approved, implement the change as planned
* If disapproved, the whole process is canceled and must be resumed if necessary
* If necessary, the approver may request additional information and/or adjustments that he/she deems necessary before approving the change

 

**Implementation**: 
After the approval of the change, the person responsible for the implementation must perform the necessary procedures to ensure that the planned steps are carried out.
If the change is successfully implemented, notify involved parties and close the process.
If the change was not successfully executed, trigger the rollback plan.
