# API Exploration Scripts

This repository contains several scripts and Jupyter Notebook examples for exploring public APIs related to New Zealand's electricity market, electric vehicle data, land information, and demographic data from Stats New Zealand. These demonstrate how to fetch, process, and analyze data from various APIs. They are intended for developers, data analysts, or anyone interested in energy, transportation, geospatial data, and demographic statistics in New Zealand.

## Included Notebooks and Scripts

### 1. `emi-api-test.ipynb`

Focuses on the Electricity Market Information (EMI) API for real-time electricity dispatch data.

### 2. `homeiq-api-exploration-test.ipynb`

Explores the NZTA EV API for electric vehicle registration and specifications data, as well as the LINZ API for land information and geospatial data queries.

### 3. `fetch_nz_addresses.py`

Python script to fetch New Zealand address data using LINZ WFS API.

### 4. `statsnz_api_call.py`

Python script to fetch demographic and population data from Stats NZ API.

All notebooks and scripts use Python and libraries such as `urllib`, `json`, `requests`, `geopandas`, and `pandas` for data handling, and include example code for API requests, data filtering, calculations, and basic analysis.

---

## Prerequisites

* **Python 3.6+** installed.
* **Jupyter Notebook or JupyterLab** (`pip install notebook`).
* **Required libraries** (`requests`, `pandas`, `geopandas`):

```bash
pip install requests pandas geopandas
```

* **API Keys:**

  * EMI API key: Obtain from the [EMI developer portal](https://emi.azure-api.net).
  * LINZ API key: Obtain from the [LINZ Data Service portal](https://data.linz.govt.nz).
  * Stats NZ API key: Obtain from the [Stats NZ Data Service](https://data.stats.govt.nz/).

* Internet access for API calls.

---

## Setup Instructions

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open your desired notebook or script (`emi-api-test.ipynb`, `homeiq-api-exploration-test.ipynb`, `fetch_nz_addresses.py`, or `statsnz_api_call.py`) and run sequentially. Modify API keys, URLs, or parameters as needed.

---

## Script Details

### EMI API Test (`emi-api-test.ipynb`)

Interacts with the Electricity Authority's EMI API to retrieve real-time dispatch data for New Zealand's electricity market.

### HomeIQ API Exploration Test (`homeiq-api-exploration-test.ipynb`)

Explores NZTA API for EV/PHEV vehicle data (from 2020 onwards) and LINZ API for geospatial data.

### Fetch NZ Addresses (`fetch_nz_addresses.py`)

Script to fetch New Zealand address data from LINZ using the Web Feature Service (WFS) API.

### Stats NZ API Call (`statsnz_api_call.py`)

Script to fetch demographic and population data from Stats NZ.

**Key Features:**

* Fetches demographic data from Stats NZ APIs.
* Easily customizable for specific data queries.

**Usage Example:**

* Set your API key in the script.
* Execute the script to retrieve demographic data.

**Sample Output:**

* JSON data displaying demographic details.

*Note:* You can always generate free API keys and monitor API rate limits.

---

## Running the Notebooks and Scripts

* Notebooks contain markdown explanations and executable code cells.
* Adjust variables (API URLs, keys, filters) as necessary.
* For continuous monitoring (`emi-api-test.ipynb`), uncomment and adjust the loop timing carefully.

---

## Limitations and Notes

* Scripts are exploratory with basic error handling.
* API data sources may change; refer to respective API documentation.
* No built-in data visualization (extendable with libraries like Matplotlib).

---