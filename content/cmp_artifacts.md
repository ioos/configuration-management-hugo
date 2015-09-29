+++
weight = "40"
type = "post"
draft = false
sidebar = true
Title = "IOOS DMAC CMP Artifacts"
+++



# RECOMMENDED CONFIGURATION 

The table below defines the configuration and processes that should be followed by all IOOS data providers.

## Data Server Software
--------------------

Below is the table of data server software and specifications that should be deployed for IOOS data providers.

| Data server software| IOOS Recommended Version |
|:--- |:--- |
|i52N SOS|[1.0.0](https://github.com/ioos/i52n-sos)|
|ncSOS|[v1.2](https://github.com/asascience-open/ncsos) for TDS versions 4.5 and 4.6, or [v1.1](https://github.com/asascience-open/ncsos)</u> for older TDS versions|
|WMS|[1.3.0-http://www.opengeospatial.org/standards/wms][-http://www.opengeospatial.org/standards/wms]|
|THREDDS|any version starting with [4.3.16-http://www.unidata.ucar.edu/blogs/news/entry/netcdf_java_library_and_tds1]; [4.6-http://www.unidata.ucar.edu/software/thredds/v4.6/tds/UpgradingTo4.5.html] /Java 8 preferred|
|ERDDAP|at least [1.62-http://coastwatch.pfeg.noaa.gov/erddap/download/setup.html];[1.64-http://coastwatch.pfeg.noaa.gov/erddap/download/setup.html]/Java 8 preferred</u>|


### Service Configuration and Registration

There are three options for IOOS data providers for registration of their data services and interface to the IOOS Catalog.

1.  **Preferred method:** IOOS data provider establish and run an instance of the OGC Catalog Service (CSW), to allow for federation with other services. There are tw


|   S/W     | Version|
|-------|-----|
| CSW (standard version)   | 2.0.2 |
| pyCSW                    | 4.3   |

Must have WAF (minimum requirement). Track location – manual.

And/or CSW

# CONFIGURATION BASELINE

Where does partner config info come from? A) Catalog for Data Server software version, b) Standard spec version, c) Service URLs

|                   |                                    |                                   |
|-------------------|------------------------------------|-----------------------------------|
|                   | **Services/Datasets (Do we just point to Catalog?)** | **Assets (from Asset Inventory)** |
| **Data Provider** | **SOS**                            | **THREDDS**                       |
| AOOS              |                                    |                                   |
| CeNCOOS           |                                    |                                   |
| CARICOOS          |                                    |                                   |
| More RA’s…        |                                    |                                   |
| NDBC              |                                    |                                   |
| CO-Ops            |                                    |                                   |
| HFR DAC           |                                    |                                   |
| GLIDER DAC        |                                    |                                   |
| ATN               |                                    |                                   |


# AVAILABLE SERVICES AND DATASETS

## IOOS Catalog Dataset/Services counting

* Luke and Kelly on the API for that.

## Asset Inventory

* Kathy is working on Mooring Management Plan

* More sources of data for Asset Inventory

  - Catalog (based on registration). Webservice URL downloads from Luke.

  - Annual submission by RAs (ground truth for Catalog data)

  - John TenHoeve stuff (2 years old)

  - ???
