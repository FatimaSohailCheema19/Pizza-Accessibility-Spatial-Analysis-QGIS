# 🍕 Pizza Accessibility Spatial Analysis using QGIS

A geospatial analysis project developed in **QGIS** to study pizza accessibility using spatial buffers, intersections, and census block-group data.

The project demonstrates how GIS techniques can be used to evaluate the geographic accessibility of pizza locations and visualize areas that fall within a defined service or accessibility distance.

---

## 📌 Project Overview

Geographic Information Systems can be used to analyze how easily people can access services, businesses, and facilities based on location.

In this project, QGIS was used to perform a spatial accessibility analysis using:

- Pizza location data
- Census block-group data
- 500-meter buffer zones
- Spatial intersection
- GeoPackage layers
- Map visualization

The goal was to identify geographic areas located within a specified distance of pizza locations and create a final map showing the spatial relationship between those areas.

---

## 🎯 Objectives

The main objectives of this project were to:

- Work with geospatial vector data in QGIS
- Understand the use of buffer analysis
- Perform spatial intersection
- Analyze accessibility based on distance
- Work with census block-group boundaries
- Create and manage GeoPackage layers
- Produce a final spatial visualization
- Gain practical experience with GIS-based spatial analysis

---

## 🛠️ Tools & Technologies

- QGIS
- Geographic Information Systems (GIS)
- GeoPackage
- Spatial Buffer Analysis
- Spatial Intersection
- Vector Layers
- Map Visualization
- Geospatial Data Analysis

---

## 🗺️ Spatial Analysis Workflow

The project follows the general workflow:

**Load Spatial Data → Prepare Geographic Layers → Create 500 m Buffers → Perform Spatial Intersection → Analyze Accessible Areas → Create Final Map**

---

## 📍 Geographic Data

The analysis uses several geospatial layers representing geographic boundaries and pizza accessibility results.

The main spatial files included in this repository are:

- `NH_BlockGroups_Clipped.gpkg`
- `Pizza_Buffer_500m.gpkg`
- `Pizza_Access_Intersect.gpkg`

Each GeoPackage represents a different stage of the spatial analysis.

---

## 🧱 Census Block Groups

The file:

**data/NH_BlockGroups_Clipped.gpkg**

contains the clipped census block-group layer used as the geographic base for the analysis.

Block-group polygons provide the spatial units required to evaluate which geographic areas overlap with pizza accessibility zones.

---

## 📏 500-Meter Buffer Analysis

A buffer was created around pizza locations using a distance of:

**500 meters**

Buffer analysis creates a geographic zone around each pizza location.

These zones represent areas considered to be within the defined accessibility distance.

The resulting buffer layer is stored as:

**data/Pizza_Buffer_500m.gpkg**

---

## 🔀 Spatial Intersection

After creating the pizza buffers, an intersection operation was performed between the buffer zones and the census block-group layer.

This operation identifies portions of geographic areas that overlap with pizza accessibility zones.

The resulting layer is stored as:

**data/Pizza_Access_Intersect.gpkg**

---

## 🧠 Why Use Spatial Intersection?

Spatial intersection combines geographic features that occupy the same physical space.

In this project, it helps answer questions such as:

- Which block-group areas fall within pizza accessibility zones?
- Which geographic areas overlap with a 500-meter pizza buffer?
- How can accessibility be represented spatially?
- Which regions appear to have greater or lower access?

---

## 🗺️ Final Map

The project includes a final exported map:

**map/Pizza_Map.png**

The map visually presents the results of the spatial accessibility analysis.

A corresponding world file is also included:

**map/Pizza_Map.pgw**

The `.pgw` file stores georeferencing information associated with the PNG map image.

---

## 📁 Repository Structure

Pizza-Accessibility-Spatial-Analysis-QGIS/

├── data/

│   ├── NH_BlockGroups_Clipped.gpkg

│   ├── Pizza_Access_Intersect.gpkg

│   └── Pizza_Buffer_500m.gpkg

│

├── map/

│   ├── Pizza_Map.png

│   └── Pizza_Map.pgw

│

├── screenshots/

│   ├── QGIS project setup

│   ├── Geographic layers

│   ├── Buffer creation

│   ├── Buffer results

│   ├── Spatial intersection

│   ├── Attribute analysis

│   ├── Map styling

│   └── Final map output

│

├── report/

│   └── Pizza_Accessibility_Spatial_Analysis.docx

│

└── README.md

---

## 📸 Screenshots

The **screenshots/** directory documents the major stages of the QGIS workflow.

The screenshots include examples of:

- Opening the QGIS project
- Loading geographic data
- Viewing census block groups
- Creating pizza accessibility buffers
- Inspecting buffer results
- Performing spatial intersection
- Examining output attributes
- Styling map layers
- Preparing the final visualization

These screenshots provide step-by-step evidence of the spatial analysis process.

---

## 📄 Project Report

The complete project report is available in:

**report/Pizza_Accessibility_Spatial_Analysis.docx**

The report documents the GIS workflow and the spatial analysis performed during the assignment.

---

## 🔎 Main GIS Techniques Used

### Buffer Analysis

Buffering was used to create a fixed-distance accessibility zone around pizza locations.

This converts individual location features into geographic areas that can be compared with other spatial layers.

---

### Spatial Intersection

Intersection was used to combine overlapping portions of the pizza buffer and block-group layers.

This produced a new spatial layer representing areas that satisfy both geographic conditions.

---

### Layer Management

Different spatial layers were organized and managed within QGIS to separate:

- Base geographic data
- Buffer results
- Intersection results
- Final visualization

---

### Map Visualization

The final results were visually represented using QGIS map styling and export tools.

Map visualization makes spatial relationships easier to understand than examining attribute tables alone.

---

## 💡 Applications of Accessibility Analysis

The same GIS workflow can be applied to many real-world problems, including:

- Restaurant accessibility
- Hospital coverage
- School accessibility
- Public transportation coverage
- Retail location analysis
- Emergency-service coverage
- Delivery zones
- Urban planning
- Facility placement
- Service-area analysis

---

## 🧠 Key Learning Outcomes

Through this project, I practiced:

- Working with QGIS
- Loading vector data
- Managing GeoPackage files
- Understanding spatial relationships
- Creating distance buffers
- Performing spatial intersection
- Working with geographic boundaries
- Inspecting attribute data
- Styling GIS layers
- Exporting maps
- Understanding accessibility analysis

---

## 🚀 Possible Future Improvements

This project can be extended through:

- Comparing multiple buffer distances
- Adding population information
- Calculating the percentage of each block group within an accessibility zone
- Performing network-based accessibility analysis
- Comparing different restaurant categories
- Adding demographic information
- Creating an interactive GIS dashboard
- Performing density analysis
- Identifying underserved geographic areas
- Using travel-time instead of straight-line distance

---

## 🎓 Academic Context

This project was completed as part of a **Data Visualization / GIS practical assignment**.

The objective was to gain hands-on experience with spatial data, QGIS tools, buffer analysis, spatial intersection, GeoPackage layers, and map-based visualization.

---

## 👩‍💻 Author

**Fatima Sohail**

BS Data Science  
GIFT University

---

## ⭐ Support

If you find this GIS project useful for learning QGIS, spatial analysis, or accessibility mapping, consider giving the repository a ⭐.
