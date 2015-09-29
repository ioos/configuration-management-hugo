+++
weight = "20"
type = "post"
draft = false
sidebar = true
Title = "IOOS DMAC Configuration Management (CM) Plan"
+++






_This Configuration Management Plan (CM Plan) is a tool used to establish the overall approach for the Configuration Management Process requirements for the DMAC implementation. The scope of this plan extends to software components of the DMAC infrastructure, and includes an accounting of deployed IOOS assets.  The CM Plan is a dynamic compound document, with a static part incorporated herein, and a dynamic part is published as a separate ["IOOS DMAC CMP Artifacts"](/cmp_artifacts/) document._
<!--more-->


# Purpose


The purpose of this Configuration Management Plan is to describe the process by which IOOS will

-   Define the software and standards versions recommended for deployment by data provider partners

-   Identify the configuration of deployed IOOS DMAC components at given points in time

-   Systematically communicate recommended changes to the configuration, and control the deployment of those changes

-   Maintain the integrity and traceability of the configuration over time

-   Provide an accounting of deployed IOOS assets, including services and datasets, over time

The IOOS CM Plan is a living document that identifies CM roles and responsibilities, resources, and formal processes and procedures to ensure that all proposed changes to major DMAC components and applications are evaluated and approved before implementation.  This plan is essential for effective CM pertaining to activities such as system-wide upgrades, replacements, and deployments.  In addition, it is a key process for maintaining the appropriate level of information assurance for DMAC implementation.

# Scope
 
The Configuration Management aspect of this plan covers specific components of the IOOS DMAC infrastructure, including:

1.  IOOS DMAC data server software packages (e.g. ncSOS, i52N)

2.  Standards adopted or recommended by IOOS DMAC (e.g. OGC SOS, THREDDS, CS/W)

This plan also endeavors to maintain an accounting of deployed IOOS assets, such as data offerings from IOOS Data Providers (data providers include IOOS Regional Associations (RA’s), Federal partners (NDBC and CO-OPS) and IOOS Data Assembly Centers). Assets to be tracked include:

1.  Number of services

2.  Number of data sets

3.  Number of stations/platforms/sensors

# Responsibilities and Authority

Establishment of this CM Plan is the responsibility of the IOOS Program Office, using inputs from stakeholders. Because IOOS is a community-based endeavor, and most data providers are grant recipients (rather than contractors), the IOOS Program Office does not have the authority to mandate, or prevent, changes to systems at data provider locations. It is up to the individual provider to determine when, and if, changes should be made. However, IOOS has made, and will continue to make, investments in software packages and tools to enhance the services provided by stakeholders and will make recommendations to data and service providers in an effort to enhance exposure and use of the data.

# Configuration Management Process

The diagram below illustrates the Configuration Management process.

![IOOS CM Process](/images/process_small.png) 

<!-- <img src="/images/process.png" style="width: 50%; height: 50%"/> -->

## Configuration Management Artifacts: Current Recommendations and Configuration Management Baseline

This Configuration Management Plan is intended to be a fairly static description of the CM process. There are three related [artifacts](/cmp_artifacts/) published separately, which contain the configuration data and are intended to be references updated on a more dynamic basis.

1.  **Recommended DMAC Configuration** - defines the specific software and/or standards versions that IOOS currently recommends for data provider deployments.

2.  **Configuration Baseline** - tabulation of what is currently deployed at each data provider locations. This baseline is updated each time a data provider upgrades services.

3.  **Available Services and Datasets** - contains a summary of the services and datasets available from each data provider at a given points in time.

