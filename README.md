# trees4uucl
A repo for documenting the creation of a tree inventory on the property of UUCL Kentucky.

<!-- TOC -->

## Table of Contents
- [Part I. ](#part-i-project-summary-proposal)  
- [Part II. ](#part-ii-data-sources)  
    - [Basemap Data](#basemap-data)
    - [Census Bureau Tracts](#census-bureau-tracts)
- [Part III. Proposed Visuals](#part-iii-proposed-visuals)
- [Part IV. Objectives and User Needs](#part-iv-objectives-and-user-needs)
- [Part V. Data Processing and Storage](#part-v-data-processing-and-storage)
- [Part VI. Data Stack and JS Libraries to Employ](#part-vi-data-stack-and-js-libraries-to-employ)
- [Part VII. Layout](#part-vii-layout)
- [Inspiration](#inspiration)
- [References for readme](#references-for-readme)  
- [Final Map](#Final-Map)

<!-- /TOC -->

## Part I: Project Summary Proposal
Create two map types:
1. The utilization by 7 Acres Committee to monitor and maintain their tree inventory.
2. The utilization by general members and the public to walk the grounds and identify tree by common name.

## Part II: Data Sources
### Basemap Data
Could use data from KYFromAbove N095E297 quadrant

### UUCL Tree Inventory Aug 2022
UUCL 7 Acres Committee provided csv containing tree information from Tree Inventory performed on March 25- 26 & April 8 2022. Data file contains the following attributes:
- Zone on property where tree exists
    1. Memorial Garden
    2. Woods
    3. Front Lawn
    4. Back Corner
- Tree ID# (unique for every tree identified)
- Cirumference (feet & inches)
- Diameter at Breast Height (DBH) (calculated by dividing circumference by 3.1415 to convert)
- Structure
    - Good
    - Moderate
    - Poor
- Health 
    - Good
    - Moderate
    - Declining
    - Dead
- Date of Planting
- Hazard/Safety Risk that may apply to tree
    - Deadlimbs
    - Standing Dead
    - Decay on Trunk
    - Dead tree/branches over trail
    - Parking underneath
- Maintenance Recommended
    - Cut Down
    - Cut Grape vines
    - Monitor Health
    - Remove Wire and POsts
    - Prune crossing/rubbing limbs
    - Mulch over roots
    - Monitor for Emerald Ash Borer (EAB)
- Any additional Notes

A kmz file was also provided with the points representing each tree and only it's corresponding ID # as 'Name' attribute.


## Part III. Proposed Visuals
Map Layer with color coded system for maintenance and priority of action
    - red = high priority
    - orange = medium priority
    - yellow = low priority
    - green = no reponse needed at this time
Could make into an interactive web map, allow pin pointing user location to help them identify where on the property they are with respect to the trees.


## Part IV. Objectives and User Needs
Visitor Use:
    - Tree ID 
    - Identify Differences Between Trees using Common Name
Maintenance Use: 
    - Tree ID 
    - Health 
    - Maintenance Recommendations
    - Hazard/Safety



## Part V. Data Processing and Storage
Import kmz into QGIS and export as geojson
Since the excel file contained data with more detail beyond Tree ID# will need to merge the data of interest from csv to the point geojson.

## Part VI. Data Stack and JS Libraries to Employ


## Part VII. Layout
### Mockup WireFrame 1

## Inspiration
Health of Tree Inventory for 7 Acres Committee Use inspired by Illinois [Chapter Community Associtations Institute](https://www.cai-illinois.org/tree-inventory-community-benefits-seeing-forest-trees/).

## References for readme

## Final Map