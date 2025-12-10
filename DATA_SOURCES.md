# Data Sources Documentation

This document provides details about the datasets used in the Vancouver Business Heritage Proximity Predictor project.

## Date of Download
December 9, 2025

## Datasets

### 1. Business Licences Dataset

**Source:** City of Vancouver Open Data Portal
**URL:** https://opendata.vancouver.ca/explore/dataset/business-licences/
**Download Link:** https://opendata.vancouver.ca/explore/dataset/business-licences/download?format=csv
**File Location:** `data/raw/business_licences.csv`

**Description:**
Business licence records from 2024 onwards with streamlined business categories. The extract for business licences of the current year is updated daily. Effective May 6, 2024, the City streamlined its business licence categories, consolidating over 500 categories into fewer than 100.

**License/Terms of Use:**
Open Government Licence - Vancouver
https://opendata.vancouver.ca/pages/licence/

**Dataset Statistics:**
- Number of records: 132,635 businesses
- Number of columns: 25
- File size: ~33.2 MB

**Key Columns:**
- `licencersn`: License reference serial number
- `licencenumber`: License number
- `businessname`: Legal business name
- `businesstradename`: Trade name
- `status`: License status
- `issueddate`: Date license was issued
- `expireddate`: Date license expires
- `businesstype`: Type of business (streamlined categories)
- `businesssubtype`: Subtype of business
- `house`: Street number
- `street`: Street name
- `city`: City
- `province`: Province
- `postalcode`: Postal code
- `localarea`: Vancouver local area/neighborhood
- `geom`: Geometry field
- `geo_point_2d`: Geographic coordinates (latitude, longitude)

**Geographic Coverage:**
All businesses contain geographic coordinates in the `geo_point_2d` field.

---

### 2. Heritage Sites Dataset

**Source:** City of Vancouver Open Data Portal
**URL:** https://opendata.vancouver.ca/explore/dataset/heritage-sites/
**Download Link:** https://opendata.vancouver.ca/explore/dataset/heritage-sites/download?format=csv
**File Location:** `data/raw/heritage_sites.csv`

**Description:**
A listing of buildings and structures, streetscapes, and landscape resources (parks and landscapes, trees, monuments, public works) which have been deemed to have heritage value. The dataset contains data on sites listed on the Vancouver Heritage Register by the following categories: Heritage Buildings, Heritage Streetscapes, Heritage Landscape Resources including Monuments, Trees, and Parks & Landscapes.

**License/Terms of Use:**
Open Government Licence - Vancouver
https://opendata.vancouver.ca/pages/licence/

**Dataset Statistics:**
- Number of records: 2,495 heritage sites
- Number of columns: 20
- File size: ~592 KB
- Update frequency: Updated annually

**Key Columns:**
- `id`: Unique identifier
- `streetnumber`: Street number
- `streetname`: Street name
- `additionallocationinformation`: Additional location details
- `category`: Heritage category (Building, Streetscape, Landscape Resource)
- `buildingnamespecifics`: Specific building name or details
- `evaluationgroup`: Evaluation group classification
- `municipaldesignationm`: Municipal designation (M)
- `provincialdesignationp`: Provincial designation (P)
- `heritagerevitalizationagreementh`: Heritage Revitalization Agreement (H)
- `interiordesignationi`: Interior designation (I)
- `landscapedesignationl`: Landscape designation (L)
- `heritageconservationareaca`: Heritage Conservation Area (CA)
- `heritageconservationcovenanthc`: Heritage Conservation Covenant (HC)
- `federaldesignationf`: Federal designation (F)
- `status`: Current status
- `dateoflastupdate`: Date of last update
- `localarea`: Vancouver local area/neighborhood
- `geom`: Geometry field
- `geo_point_2d`: Geographic coordinates (latitude, longitude)

**Geographic Coverage:**
All heritage sites contain geographic coordinates in the `geo_point_2d` field.

---

## Data Quality Notes

Both datasets include:
- Valid geographic coordinates (latitude/longitude) for spatial analysis
- Local area (neighborhood) information
- Address information (street number, street name)

## License Summary

Both datasets are available under the Open Government Licence - Vancouver, which allows:
- Commercial and non-commercial use
- Modification, incorporation into other products
- Distribution

**Attribution Required:**
Contains information licensed under the Open Government Licence – Vancouver.

## Next Steps

For data preprocessing and feature engineering, refer to [PROJECT_PLAN.md](PROJECT_PLAN.md) Task 2.
