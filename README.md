# Case Study: Ensuring Election Integrity

In the recently concluded election, the Independent National Electoral Commission (INEC) has faced multiple legal challenges concerning the integrity and accuracy of the election results. Allegations of vote manipulation and irregularities have been widespread, prompting a thorough investigation into the matter.
Your mission, should you choose to accept it, is to help us uncover potential voting irregularities and ensure the transparency of the election results. You will achieve this by identifying outlier polling units where the voting results deviate significantly from neighbouring units, indicating potential influences or rigging. Your keen analytical skills and attention to detail will be critical in this endeavour.

## Task Overview
In this stage, you will focus on identifying outlier polling units based on the votes each party received. The analysis will involve geospatial techniques to find neighbouring polling units and calculate an outlier score for each party in each unit. The goal is to pinpoint polling units where the voting results significantly deviate from their neighbours, indicating potential irregularities or influences.

## Task Objectives
### 1. Dataset Preparation:
- Open the [drive link](https://drive.google.com/drive/folders/173oHgms6wYy5WKz_i3Lhl5mXcmobCWHz) and find your state of origin. If you are not a Nigerian, pick a random state.

- Download the {YOUR_SELECTED_STATE}_crosschecked spreadsheet or CSV file.
- If your selected dataset does not include longitude and latitude values for each polling unit or ward, use geocoding techniques to obtain them.

### 2. Neighbour Identification:
- Identify neighbouring polling units based on geographical proximity. Define a radius (e.g., 1 km) to determine which units are considered neighbours.

### 3. Outlier Score Calculation:
- For each polling unit, compare the votes each party received with those of its neighbouring units.
- Calculate an outlier score for each party based on the deviation of votes from neighbouring units.
- Record the outlier scores along with the respective parties and neighbouring units.

### 3. Sorting and Reporting:
- Sort the dataset by the outlier scores for each party to identify the most significant outliers.
- Provide a detailed report explaining the methodology and findings.
- Highlight the top 3 outliers and their closest polling units, explaining why they are considered outliers.
  
#### Tips
5. You can use geocoding techniques such as Google Maps Geocoding API or OpenCage Geocoding API, and add the geospatial data to the dataset.
6. You can use geodesic distance to calculate the distance between each polling unit and all other units, and set a predefined radius (e.g., 1km).
6. For each polling unit, calculate the difference in votes for each party compared to the votes of its neighbouring units and calculate an outlier score for each party as the absolute difference between the unit’s votes and the votes of its neighbours.
7. Visualize the results using maps and charts where appropriate.
