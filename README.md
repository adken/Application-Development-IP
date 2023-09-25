## PLUS Software Development IP
### Software Development Application Development Object-based Image Analysis
![Adriko_Proposal_001](https://user-images.githubusercontent.com/29119766/173377563-0d38b8b1-a02b-42f1-9210-2fc5ad4a8e2e.png)

#### Steps
- Implement image import and band selection
  - Image import 
- Implement index calculation
     -  User option to select image bands/layers for specific bands
     -  Execute button to calcalute index
     
- Indices

  - Normalized Difference Vegetattion Index (NDVI) (nir - red)/(nir + red) <br>
    The value of NDVI ranges between -1.0 to +1.0. The NDVI values near +1.0 (usually (0.6 to 0.9) indicate the dense vegetations; the negative values -1.0 to near 0         represents clouds, water, and snow; values near zero to 0.1 means barren rock, sand, or snow; moderate NDVI values +0.2 to +0.5 indicate sparse vegetations such as       shrubs and grasslands or senescing crops.
    
  - Normalized Difference Builtup Index (NDBI) (swir - nir )/(swir + nir ) <br>
    The Normalized Difference Built-Up Index is used to extract the built-up areas in urban areas automatically.
    
  - Normalized Difference Water Index (NDWI) (nir - swir)/ (nir + swir) <br>
    The Normalized Difference Water Index (NDWI) measures the change in water content of leaves using near-infrared (NIR) and short-wave infrared (SWIR) wavelengths,         NDWI is used to analyze vegetation's water content because of its sensitivity to the water content of vegetation and water bodies. 
    
  Source: https://www.gis-tutorials.net/blog/remote-sensing-indices-and-their-calculations-ndvi-ndwi-evi-savi-ndbi-mndwi-ibi/
    
- Implement index-based image classification using multi-threshold segmentation
  - predefine classes; water for NDWI, vegetation for NDVI, urban areas for NDBI
  - segmentation slider for respective thresholds
  - merging objects for respective classes
  - export resulting classes to vector format

