# CSF.CM: Climate Smart Forestry (CSF) Composite Mapper (CSF.CM) 
🌎⛰️🌳🌲 **CSF.CM** The Climate Smart Forestry (CSF) Composite Mapper (CSF-CM) is a user-friendly, Google Earth Engine (GEE)-based web app designed to generate composite CSF indicators using remote sensing data at scalable levels. The app allows users to combine maps from the adaptation, mitigation, and social dimensions, representing the three pillars of CSF, to evaluate the "smartness" score of the generated composite. The resulting composite indicator, scaled from 0 to 1, can be simultaneously generated for up to four geographically distant sampling areas, enabling users to assess smartness scores across different forest management contexts.
![Image](https://github.com/user-attachments/assets/6e4cb918-ec9c-4ce0-99a1-2f67dce072c2)

---
## 📚 Background and Access
CSF.CM is a GEE web app that enables users to create aggregated and overlapped CSF composites without prior coding knowledge. To access the app, open the page link in a browser (in progress).

## How to Access the GEE App
To view and interact with the GEE app, simply click the link below (in progress).
To download an example dataset for computing growing stock indicators from multiple plots in the CSF.Ind web-based app, click (in progress). 
To download the input data template for computing the CSF.Ind web-based app, click (in progress). 
For more details about the required data for the app, download the guideline document (in progress). 

Note: For a detailed description of the procedure and to view the repository, visit the project on GitHub. To learn how to use the app, watch the video tutorial (in progress).

## Logo
<div style="display: flex; justify-content: space-around; align-items: center;">
  <img src="https://github.com/user-attachments/assets/4a9a1811-4d3f-410a-acc9-6958f944c47e" alt="unimol_logo_png" width="200" />
  <img src="https://github.com/user-attachments/assets/8ceb07ba-c715-4c85-b1aa-ad20de6c8e22" alt="forwards_logo_png" width="200" />
  <img src="https://earthengine.google.com/static/images/earth-engine-logo.png" alt="geeapp_logo_png" width="200" />
</div>

## UI CSF.CM
![rs_2](https://github.com/user-attachments/assets/cb03d691-8fbf-4b08-af1b-cede16206391)

### 🚀 Overview
This web-based app is applicable to all European forest covers and is designed to support layers with different resolutions.

### 🎯 Objective
The primary objective of CSF.CM is to provide a robust and user-friendly tool for creating CSF composites using validated procedures from the Forwards project. The app aims to:
- Simplify the generation of CSF composites for users without coding expertise.
- Support decision-makers in forest management under Sustainable Forest Management (SFM) criteria.
- Align with the Climate Smart Forestry (CSF) concept.

### 📚 Reference
The computation of CSF.CM is based on geospatial datasets and validated procedures. For more details, refer to the following publication:
- Alvites, C., O'Sullivan, H., Francini, S., Marchetti, M., Santopuoli, G., Chirici, G., ... & Bazzato, E. (2025). Canopy Height Mapper: A Google Earth Engine application for predicting global canopy heights by combining GEDI with multi-source data. Environmental Modelling & Software, 183, 106268.

### 👨‍💻 Developers
Alvites Cesar  
Post-Doctoral Researcher, University of Molise  
Email: calvites1990@gmail.com  

### 🙏 Acknowledgments
This web-based app was developed as part of post-doctoral research at the University of Molise by Cesar Alvites, within the framework of the Forwards project.
Learn more about the project: https://forwards-project.eu/

### 🛠️ CSF.CM Web Application Configuration
#### Choose CSF Pillar
Users can select between two pillars:
- **Mitigation**: Includes growing stock, carbon stock, deadwood, and other layers.
- **Adaptation**: Includes species composition, structural diversity, and other layers.

### Table 2: Climate Smart Forestry (CSF) Input Data

| CSF Pillar         | Indicator                            | Input Data                                        | Pixel-wise | Year       | Output                      |
|--------------------|----------------------------------|-------------------------------------------------|------------|-----------|-----------------------------|
|                    | **Carbon Stock**                 | Above Ground Biomass                            | 300m       | >2010     | Composite CSF index         |
|                    | **Soil Condition**               | Soil organic carbon content (g/kg)             | 250m       | <2018     |                             |
|   **Mitigation**   | **Forest Damage**                | Burned Area Pixel                              | 250m       | 2001      |                             |
|                    | **Forest Area**                  | Global Forest Change                           | 30m        | <2023     |                             |
|                    | **Tree Species Composition**     | Land Cover Type                                | 100m       | <2018     |                             |
|                    | **Naturalness**                  | Potential Natural Vegetation Biomes           | 1000m      | 2002      |                             |
|   **Adaptation**   | **Soil Condition**               | Digital Elevation Model, Slope, Aspect        | 30m        | 2015      |                             |
|                    | **Age Structure & Diameter Dist.** | Canopy height (max and SD)                   | 10m        | 2018-2023 |                             |
| **Social Dimension** | **Forest Damage**               | Global Human Modification                      | 1km²       | 2016      |                             |

#### Upload Excel File
Users can upload up to three layers (.GeoTIFF) containing the required geospatial data for the overlapped area. Refer to Table 1 in the app for specific example data requirements.

#### Requested Data
After uploading the geospatial data, the app will display available geospatial datasets from GEE (see Table 1). Users can select some of these datasets to combine with the previously uploaded layer. Layers can be selected from a drop-down menu (e.g., layer1, layer2, etc.).

#### Setting the Weight for Layers
After uploading and selecting geospatial data to combine, users can enter a weighting score for each layer in the GEE app. The default value is 1 if no modifications are made, but users can assign decimal values (e.g., 0.2 to indicate 20%).

#### Download Outputs
Users must set the path and name where the CSF composite map will be saved before clicking 'Run' to store the geospatial CSF composite data.
- **Download CSF composite (.GeoTIFF)**: Download a layer of combined maps.

#### Run Analysis
The CSF.CM analysis is automatically computed once all required inputs are provided, and the data is saved to your personal drive.

### 📜 License
This project is licensed under the GPL3 License. See the LICENSE file for details.

### 📧 Contact
For questions or feedback, please contact:  
Cesar Alvites  
Email: calvites1990@gmail.com  
GitHub: Cesarito2021  

---
