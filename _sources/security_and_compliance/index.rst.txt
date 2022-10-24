Security & Compliance
=====================

----------------
Data sovereignty  
----------------

Users’ data, including the backup system data, models and disaster recovery, are kept within Pyplan Enterprise region. There is no transfer out of the region.  

------------
Data privacy  
------------

Pyplan has created exhaustive internal processes to guarantee customer data security. 
Pyplan undertakes to protect customer data and to communicate openly and transparently. 


------------------------------------
Data Separation, storage & transport  
------------------------------------

Pyplan Enterprise is a multi-tenant platform. As a multi-tenant platform, it is crucial that each customer's data is separated from other customer's data. 
Each tenant has a working space completely isolated from other's. 
When a user logs in Pyplan, the corresponding working space is set up as a disc unit, making it impossible to move it to other working spaces.

Pyplan uses an encrypted file system, relying on the services of a leading provider such as Amazon Web Services (AWS). 
The encryption of the file system has the following features: 

- **encrypting data at rest**: The AWS key management infrastructure uses Federal Information Processing Standards (FIPS) 140-2 approved cryptographic algorithms. The infrastructure is consistent with National Institute of Standards and Technology (NIST) 800-57 recommendations. 
- **encrypting data in transit**: AWS uses TLS version 1.2 to encrypt data in transit. 
- **rotation**: AWS generates new cryptographic material for the key every year. 

Access to encrypting password management is restricted to qualified staff. 

----------------
Content Deletion 
----------------

The creation and removal of content that resides in the tenant is controlled by the customer. Content can be deleted by the customer at any time. Backups are removed after a period of time in accordance with Pyplan Cloud internal data retention policies. 


-----------------
Penetration tests
-----------------

Pyplan performs penetration tests every three month (among other tests) to guarantee all the infrastructure security. The customer can request test result reports whenever necessary. 

.. figure:: images/pentest.png


----------------------------------------------------
Data Security Breach Management Policy and Procedure     
----------------------------------------------------

This section details the requirements for identifying, assessing, remediating, reporting and recording data breaches from Pyplan server. 

Scope
-----

This procedure applies to all staff including employees, contractors, trainees and any other personnel who are granted access to Pyplan server. 


Assessment 
----------

A security incident is any event or occurrence that affects or tends to affect data protection, or may compromise the availability, integrity, and confidentiality of data. It includes incidents that would result in a data breach, if not for safeguards that have been put in place. 

A data breach happens when there is a breach of security leading to the accidental or unlawful destruction, loss, alteration, unauthorized disclosure of, or access to, data transmitted, stored, or otherwise processed. 


Notification of Breaches 
------------------------

Any person who becomes aware of a possible breach of privacy involving personal information in the custody or control of Pyplan will immediately inform Pyplan personnel through email to support@novix.com writing  its subject as “DATA BREACH WARNING”. 

In the body of the email the incident and the name of the accounts estimated to be exposed should be explained. 


Investigation Procedure
-----------------------

The investigation procedure will begin immediately after receiving notification. 

The investigation procedure includes: 

- Pyplan Access logs review to validate and confirm data breach 
- User access restriction and password reset 
- User activity logs review (IP addresses, access time, activity logs) to determine type of breach


Containing the Breach 
---------------------

Pyplan will take the following steps to limit the scope and effect of the breach. These steps will include: 

- shutting down the system that was breached 
- correcting weaknesses in security in case they exist
- stopping unauthorized access  
- restoring the system to previous status in case data was modified or deleted
- recovering the records
- close monitoring user activities to detect unusual behaviors


Reporting Breaches
------------------

After the system has been fixed and the service has been reset, it will be submitted a report informing the client the details of the event to decide any further action. 


--------------------------------------
Pyplan Cloud network security policies
--------------------------------------

In order to ensure a strong, secure foundation, Pyplan Cloud shares security responsibilities with an industry leading cloud infrastructure vendor and valued partner.
All data is stored using AWS services, in private networks that can only be accessed through the application.

All remote access to Pypan cloud infrastructure will either be through a secure VPN connection on a Pyplan owned device that has up-to-date anti-virus software. 

Remote access using VPN can only be performed from authorized IP addresses.

Users must not install network hardware or software that provides network services without IT approval.

Users must not download, install, or run security programs or utilities that reveal weaknesses in the security of a system. 

Secure remote access must be strictly controlled. Control will be enforced with Multi- Factor Authentication (MFA).

Only IT approved VPN clients may be used.


------------------
Teleworking policy
------------------

In order to ensure a strong, secure foundation, Pyplan Cloud shares security responsibilities with an industry leading cloud infrastructure vendor and valued partner.
All data is stored using AWS services, in private networks that can only be accessed through the application.

No organizational or customer data is stored in our offices. The offices are used as a work meeting point or to provide a suitable workplace.
However, we have the following policies related to teleworking:

 - The employee shall designate a workspace, within the remote work location, for placement and installation of equipment to be used while teleworking
 - The employee shall maintain this workspace in a safe condition, free from hazards and other dangers to the employee and equipment
 - All applicable policies for acceptable use, protection of member information, security, etc, shall be observed
 - Personally owned equipment may not be connected to Pyplan owned equipment
 - The employee is responsible for securing the equipment provided to the employee by the IT Department
 - The employee will not modify any equipment without written authorization from the IT Department.




