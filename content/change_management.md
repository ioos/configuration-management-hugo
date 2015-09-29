+++
weight = "10"
type = "post"
draft = false
sidebar = true
Title = "IOOS DMAC Configuration Management Process"
+++


_The Configuration Management Process provides the process for identification, approval, coordination and documentation of changes to a system baseline. Among other benefits, the Configuration Management process will help to establish ensure an orderly transition from one software/system/service version to the next, in a way that minimizes resources and disruption for all stakeholders while delivering enhanced capabilities._
<!--more-->

# Overview

It is understood that during any project, changes will be required to existing systems, services, specifications, etc to maintain or augment capabilities. The Configuration Management Process provides the process for identification, approval, coordination and documentation of changes to a system baseline. Among other benefits, the Configuration Management process will help to establish ensure an orderly transition from one software/system/service version to the next, in a way that minimizes resources and disruption for all stakeholders while delivering enhanced capabilities.

The Configuration Management Process strives to be efficient, transparent and not overly complex or burdensome.  

# Scope 

The Configuration Management Process applies to:

* The IOOS DMAC components, including software tools, systems, specifications, standards, best practices, etc that are listed in the table in Components Under DMAC Change Management.

* Changes that relate to established needs and requirements (rather than major new systems or capabilities).  Specifically, this process applies to changes that:
  - have minimal impact on other systems not under the authority of IOOS
  - are sufficiently well-defined that an adequate solution can be easily identified
  - relate to an existing requirement (i.e. is not a significant new capability or project)
  - have an available funding source with adequate funds so the change does not need to be part of the annual budget process

# Roles

Change Management Process roles are described below. Terms of Reference for each component will identify the specific individuals or organizations that fulfill these roles.

| Role | Responsibility |
|--------|---------------------|
| **Submitting Authority** | Individuals or organizations that are authorized to submit a Request for Change (RC)|
| **Change Management Analyst** | Team member that analyzes the RC, evaluates the RC against the approval criteria, identifies implementation steps and documents the results of the analysis |
| **Review Board** | Individuals or organizations that rule as to whether the RC is approved or denied |
| **Implementation Team** | Individuals or organizations responsible for executing or implementing approved RCs |
| **Configuration Baseline Owner** | Individuals or organizations that are responsible for maintaining a configuration baseline. | 

# Change Management Process

All IOOS DMAC components covered under this plan should have established baselines that are managed by the IOOS Program Office.  Each change to a baseline must be requested via the Change Management Process.  The process is described here in generic terms, specifics related to each component are contained in the Terms of Reference section.

1. **Submit Request** - A Request for Change (RC) is submitted by a designated Submitting Authority
2. **Review and Analyze** - The Change Management Analyst will review the RC according to the criteria defined in the Scope section and perform an analysis to identify implementation actions required and impacts on related systems and users.  The results of the review will be documented and provided to the Review Board.  Specifics to be documented in the analysis include:
 * Specific actions required to implement, including estimated cost and schedule
 * Impacted systems and interfaces
    - Backward compatibility issues, technical dependencies
    - Determination if change is optional for related systems
  * User impacts
3. **Approve or Deny** - The Review Board will review the analysis provided by the Change Management Analyst and determine whether to approve or deny the request.
4. **Implement** - Upon approval, the Implementation Team executes the actions required to make the change.
5. **Update baseline** - Once the RC has been implemented, the Configuration Baseline Owner is responsible for updating the baseline and notifying all stakeholders of the change.


# Components Under DMAC Change Management

The DMAC components listed in this section are covered under the Change Management Process.

## Software - Applications, Utilities and Tools

|Component|Baseline Configuration location|
|-----------------|-------------------------------------------|
|ncSOS - SOS server reference implementation|https://github.com/asascience-open/ncSOS |
|i52N - SOS server reference implementation|https://github.com/ioos/i52n-sos |
|IOOS Data Catalog|https://github.com/ioos/catalog |
|DMAC Service Registry| |
|pyoos data collection library|https://github.com/ioos/pyoos |
|Paegan| |
|Wicken|https://github.com/ioos/wicken |
|Metamap|https://github.com/ioos/metamap |
|nctoolbox| |
|sciwms| |
|UDUnits-PY| |
|Compliance Checker|https://github.com/ioos/compliance-checker |
|SOS Validation Tool| https://github.com/ioos/ioos-sos-validator |

## Documents and Specifications

|Document/Spec|Baseline Configuration location|
|----------------------|--------------------------------------------|
|IOOS DMAC SOS Milestone 1.0 Service Architecture| *to be documented |
|IOOS DMAC Data Provider Service Versions/Configurations|http://catalog.ioos.us/services/filter/none/SOS <br><br> then: <ul><li> Select Service of interest <li> Select Data Access URL <li> Search xml for “softwareVersion”; the line below will identify the **VERSION**, e.g. `<gml:version>2.0</gml:version>` </ul> **Note**: _this won’t work for services that have not been successfully harvested by the Catalog_ |
|SOS Milestone 1.0 Encoding Templates| |
|SOS Web Service Description Document| |
|Service Registration process|https://github.com/ioos/registry |
|CSV-TSV encoding specs|https://github.com/ioos/ioos-csv-tsv |
|IOOS SOS Compliance Tests|https://github.com/ioos/ioos-sos-compliance-tests |
|IOOS Convention for Observing Asset Identifiers|https://github.com/ioos/conventions-for-observing-asset-identifiers |
|Controlled vocabularies|https://github.com/ioos/vocabularies |

# Terms of Reference for Components Under Change Management

This section contains the specific change management terms and procedures for each component covered under this Change Management process.

The Terms of Reference for each component will define:

* **Roles** - specific individuals or organizations that will fulfill each role
* **Unique process requirements** - identification of any unique processes or process requirements specific to the component as well as the tools or artifacts to be used in the Change Management Process

## IOOS Data Catalog

### Roles

|Role|Individual or Organization|
|-------|-----------------------------------|
|**Submitting Authority**| <ul><li>IOOS Program Office <li>RA DMAC coordinators, other DMAC partners <li>Users (via ‘feedback’ mechanism on Catalog GUI) </ul> |
|**Change Management Analyst**|Carmel Ortiz/Alex Birger|
|**Review Board**|Lead: Derrick Snowden|
|**Implementation Team**| <ul><li>ASA, NGDC <li>DMAC data providers (potentially)</ul>|
|**Configuration Baseline Owner**|<ul><li>ASA for Data Catalog <li> NGDC for Service Registry related items </ul> |

### Required Tools and Artifacts

The primary tool to be used for CM for the IOOS Data Catalog is [GitHub repository](https://github.com/ioos/catalog):

1. Request for Change - Regardless of how the RC originates, it will be logged as a github issue in the catalog repo
  * Assign the Issue to the Milestone labeled “Requests for Change”
2. Review and analysis - The results of the review and analysis will be recorded as comments against the Issue. 
3. Approval/Denial 
  * If approved, the Issue will be moved out of the “Requests for Change” milestone and in to a release Milestone; 
  * If denied, the Issue will be closed with appropriate notes as to why it was denied.
4. Implementation 
  * Standard github mechanisms will be used to implement the change; 
  * Releases should be planned in accordance with semantic versioning practice 
5. Baseline Update - all appropriate documentation and code will be updated on github.


## SOS Reference Implementations (ncSOS, i52N SOS)

### Roles

|Role|Individual or Organization|
|----------|-----------------------|
|**Submitting Authority**| <ul><li>IOOS Program Office <li>RA DMAC coordinators, other DMAC partners </ul> |
|**Change Management Analyst**|Carmel Ortiz/Alex Birger|
|**Review Board**|Lead: Derrick Snowden|
|**Implementation Team**| <ul><li>ASA, Axiom (as appropriate, to make changes to software reference implementations) <li>DMAC data providers (to install/upgrade reference implementation software on their services)</ul>|
|**Configuration Baseline Owner**|<ul><li>ASA for ncSOS <li> Axiom for i52N <li>DMAC data providers  <li> IOOS Program Office </ul> |


### Required Tools and Artifacts

The primary tool to be used for CM for the SOS Reference implementations is github - [see component github repository list](#components-under-dmac-change-management).

1. Request for Change - Regardless of how the RC originates, it will be logged as a github issue in the appropriate repo
  * Changes can be new features or bug fixes (regardless they are Issues in github)
  * Assign the Issue to the Milestone labeled “Requests for Change”
2. Review and analysis - The results of the review and analysis will be recorded as comments against the Issue. 
3. Approval/Denial
  * If approved, the Issue will be moved out of the “Requests for Change” milestone and in to a release Milestone.
  * If denied, the Issue will be closed with appropriate notes as to why it was denied.
4. Implementation - ncSOS, i52N
  * The IOOS PO will coordinate with the appropriate vendor (ASA or Axiom) to implement the changes documented in github issues.
  * The vendor will implement the changes.
  * Standard github mechanisms (branches, commits, releases, etc) will be used to make the changes to the software package(s)
  * Testing will be performed by the IOOS PO to validates the changes have been made and the software is functioning as expected
  * Releases should be numbered in accordance with semantic versioning practice
  * Release notes should be made available on github
  * DMAC Data providers
     - Once the SOS Reference Implementation has been updated and tested, the IOOS PO will coordinate with the RAs, and other data providers if applicable, to have them update their servers to the newest version.
     - If Data Providers do not change the service URL, the service will not need to be re-registered in the Service Registry
5. Baseline Updates
  * SOS Reference Implementation - All appropriate documentation and code for will be updated on github.
  * DMAC Data Providers services - upon next successful harvest, the Catalog Services page will reflect the correct SOS Reference Implementation software baseline version installed at the data provider. 

## Encoding Templates

### Roles

|Role|Individual or Organization|
|----------|-----------------------|
|**Submitting Authority**| <ul><li> <li> <li> </ul> |
|**Change Management Analyst**|Alex Birger|
|**Review Board**|Lead: Derrick Snowden|
|**Implementation Team**| <ul><li> <li></ul>|
|**Configuration Baseline Owner**|<ul><li> <li>  <li></ul> |






### Required Tools and Artifacts

The primary tool to be used for CM 


# Sources

 * http://oss-watch.ac.uk/resources/releasemanagement
 * [NWS Change Management directive](http://www.nws.noaa.gov/directives/sym/pd01001001curr.pdf)
 * [O&M planning inputs from AGM Memo](https://docs.google.com/a/noaa.gov/document/d/1eZqU4WEu921OevuzO5Ac3bTaVl7Z8Ucc7aX0hmVpL-I/edit)



# Glossary 

|Term| Definition |
|-------|---------------|
|Baseline (or Baseline Configuration)|Information that is used as a starting point by which to compare other information.  In technical systems: the established starting point physical characteristics of a product, service, system or specification.| 
|Change Management|The process for identification, approval and coordination of changes to a system baseline.|
|Configuration | A configuration is the identified and documented functional and physical characteristics of a product, service, system or specification.| 
|Configuration Management|Tracking of revisions to a component’s baseline (design, configuration, technical specifications, etc).  Configuration management allows you to identify the current baseline for a system.|
|Release Management|The process of building, packaging and distributing software for consumption.|  


# Open Issues

1.	Where to document system baselines?  All on GitHub?
2.	Can this process be used to help provide justification for O&M expenditures?  How can we use it to educate partners regarding technology stewardship, evolution?

