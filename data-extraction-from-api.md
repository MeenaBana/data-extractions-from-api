#  Data Extraction via APIs
This report is a small description of  Data Extraction from APIs.

## Table of Contents
1. [Overview](#overview)
1. [Data description](#data-description)
1. [Downloading data](#data-downloading)


<a id="overview"></a>
## Overview
Skyss is the public authority that plans, purchases and markets the public transport services governed by the county authority in Hordaland, Norway. Skyss offers trips by light rail (Bybanen), bus, local boat and ferry throughout Hordaland.

<a id="data-description"></a>
## Data description
Various datasets are available through the [**Skyss Public API**](https://skyss-public-api-test.azurewebsites.net/index.html).
Descriptions of the variables and fields is available on the API website.
Following datasets are currently available:
1. Calender
2. Lines
3. Routes
4. Stop Points
5. Trips information (raw & aggregated)

<a id="data-downloading"></a>
## Data downloading
- Made single and multithreaded API requests to download various public transport data using Python and Postman. 
- Read different file formats using dask.
- **Trips Data** is very large and granular, so created day wise csv/parquet files.
- **Stop Points** and **Lines** data.