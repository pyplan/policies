.. Pyplan documentation master file, created by
   sphinx-quickstart on Tue May 24 11:53:29 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. figure:: images/logo.png
   :width: 300

.. toctree::
   :hidden:
   :caption: Content
   :titlesonly:

   pyplan_cloud/index
   deployments/index
   datasources/index
   access_management_policy/index
   security_and_compliance/index
   disaster_recovery/index
   development_process/index
   human_resources/index
   faq/index

=================================
Pyplan data and security policies
=================================



About Pyplan 
============


Pyplan is the unique Corporate Performance Management (CPM) platform integrating Data Analytics and Business Planning powered by Python.   

It allows the integration of every analytical task that supports corporate decision making in a single place such as: automatically feed off disparate data sources, monitor any key performance indicator, infer trends using self-calibrated predictive models, and simulate impacts across the enterprise to discover the best course of action.   

Pyplan is built-on top of the open source technologies that are conducting the data analytics revolution running on Python: Pandas, Numpy, Dask, SciKit-learn, to name a few of them.  

It supports a full range of users and unlimited use-cases from data collection to decision making: data gathering automation, self-service analytics, interactive dashboards, business planning, simulation and optimization, coordinated data visualization, reporting and collaboration.  



Embracing Python benefits
-------------------------

Python has become the most used programming language in the world. The level of innovation and resources (libraries) produced by its open source community can not be matched by any single company running on proprietary software. Using Pyplan, your team will be kindly introduced to start speaking the “Lingua Franca” of Data Science, Python.  

Pyplan offers cutting-edge performance, scalability and governance, with the convenience of SaaS or on-premise deployment and it is specifically designed for business users (no code – low code).  



Pyplan Enterprise SaaS Overview
===============================

Pyplan Enterprise is a native cloud platform working in a server-client architecture that can be contracted as a service running on Pyplan Cloud Infrastructure or deployed on-premise over customer’s infrastructure.  

Pyplan Cloud solution offers businesses a world-class analytics and planning platform without the complexities of installing and managing their own deployment.  

We also understand that some businesses prefer to manage their systems running on their own infrastructure. Pyplan Enterprise is also offered to be installed on customer’s infrastructure attending Pyplan requirements.  



Pyplan apps 
===========

A single platform for Data Analytics and Business Planning  
----------------------------------------------------------

.. figure:: images/pyplan-gbd.png


Pyplan Enterprise allows to host different types of applications (apps) on a single hub. Users create, collaborate and share their insights through apps specifically developed to attend different business cases.  

Applications contain all the data, business rules and documentation, providing a single portal for your users to consume all your analytics, planning and reporting assets.   


In-memory apps 
--------------

Pyplan apps are composed of two main types of assets: Business Logic and User Interfaces.  

In addition to that, you can find data extraction, transformation and  loading (ETL) processes automation, input forms, user roles and permissions settings.  


Business Logic  
--------------

.. figure:: images/pyplan-logic.png

Pyplan organizes business logic rules in a workflow represented as a hierarchical navigable influence diagram. This way of organizing code presents multiple benefits compared to traditional integrated development environments (IDEs):  

- Facilitates the understanding of the logic from a general to a detailed point of view. 
- Makes it easy to run any intermediate calculation and explore results as tables or graphs. 
- Makes it easy to test and tune the app to improve performance. 

Pyplan logic is run “on the fly” and data is stored **in-memory** on a workspace created for the user. Pandas dataframes, Numpy arrays and Xarray data-arrays are native objects used for that purpose, but since there is a Python engine running underneath, the user can decide to use any type of object that could better suit for the application purpose. For example, in case you are manipulating geo-data, it is probable you will use Geopandas objects or,  in case you need to deal with big data, it is probable you will use Vaex or PySpark objects.  

All dependencies are automatically calculated ensuring a single result no matter the calculation sequence the user triggers. This is a big differentiation from traditional **Jupyter Notebooks**.

In case a node pulls information from any external data source, it will be automatically run. There is a Python connector for almost every single data source known which makes integrating a Pyplan application with legacy systems a simple process. That is one of the unmatchable benefits of standing on top of the most innovative data analytics community.


User Interfaces
---------------

Access to Pyplan SaaS environment is through a web browser interface, known as Pyplan Cloud. The Pyplan web browser interface makes all aspects of development, drag-and-drop content creation and consumption possible.  

Pyplan features a responsive design methodology to automatically display and resize visualizations with the appropriate layout and information to fit the device — whether it is a browser on a laptop or desktop, tablet, or smartphone. Built with current standards of modern applications (React, Material Design and web sockets), Pyplan enables you to build and consume apps on any device. 


Pyplan apps devops 
------------------
 
**Move apps through a development lifecycle, not development servers**

  
In a traditional Analytics and Planning environment, apps would be developed on a development server. Once the development is completed, they would be moved to a test server. Issues found in testing would mean several iterations of this process until the application could be deployed to production, requiring a lot of resources and infrastructure to manage.  

With Pyplan Cloud SaaS, apps are stored in separate workspaces. Each workspace has its own security settings, data connections, file storage and runs on its own instance. Customers can create as many development, test and production workspaces as needed to suit their software development life cycle. This approach allows much greater agility and flexibility and reduces infrastructure expenses compared to a traditional on-premise setup.  

.. figure:: images/app-cycle.png

In the above example, users consume the app in the Public (production) workspace. When a change to the app is requested, a copy is made in the user/users (development) workspace. After consolidating changes, the candidate app is published to the Team (test) workspace for review. Several cycles may occur until the app is ready to be released to production.  

To facilitate these flows, each space has its own data connections and file storage, so that an app will load and run the appropriate data for the applicable life-cycle phase.     