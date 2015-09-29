+++
weight = "0"
type = "post"
draft = false
sidebar = true
Title = "ABOUT: IOOS Configuration Management Process"
+++

<!-- For a single homepage put in FrontMatter url = "index.html" -->

_Configuration management (CM) is a systems engineering process for establishing and maintaining consistency of a product's performance, functional and physical attributes with its requirements, design and operational information throughout its life._
<!--more-->

# Configuration Management Process

CM is defined as the systematic identification, documentation, and control of system elements by recording and reporting change processing and implementation status.  These activities assist in verifying compliance with specified system requirements as well as establishing and maintaining the technical integrity of a system throughout its life cycle.  The successful implementation of CM activities results in an established and documented system baseline , effective management and tracking of changes made to system parts and related documentation (version control), and effective risk management.

# Configuration Management Plan

Based on the United States Office of Management and Budget (OMB) circular A-130 and other Federal laws and regulations, a CM process must be developed and documented in a CM Plan for all major applications and components of the developed systems. Developing a CM Plan is critical for implementing CM and ensures the following:

* _**Changes to the configuration are identified and evaluated to determine the impact to the system before implementation.**_

Any changes made to the system are documented and tracked.  Because each change is tracked from initial system development through completion, a thorough history of changes is created for that system.  For example, the IOOS RA THREDDS Catalog running on a THREDDS Server (TDS) may require an upgrade to a more recent version of TDS because of existing vulnerabilities in the older version.  Upgrading to the more recent version of TDS will change the RA’s configuration.  The need for a version upgrade is a configuration change that must be thoroughly analyzed, since it may affect security, system performance, and functionality.  This change should be documented in a formal process to provide a historical representation of one of the changes occurring throughout the system development life cycle (SDLC).

* _**Configuration is documented ensuring that version control is maintained.  Upgrades and additions are easily implemented because of relevant controls in a formal CM process.**_

The DMAC documentation includes information on the system specification and configuration design, ensuring that, as part of the CM Plan, system documentation can be checked to verify whether the designed configuration allows the system to achieve its objective.  For example, if the IOOS Catalog design needs to be modified to implement a password for users, it could be determined that this change will be included in a later version. 

* _**The configuration is verified against the initial baseline ensuring that all changes have been maintained and documented for any new parties involved in the CM process.**_

Information on the DMAC systems, including the software types and versions, is recorded and tracked, ensuring access to the most recent system information.

A CM Plan includes and addresses CM roles and responsibilities, communications, system configuration baseline, configuration control process, and CM resources. 






