AgriWater Flow: CropWAT-Based Irrigation Manager

AgriWater Flow is a precision agriculture web application designed to digitize the   FAO CropWAT 7.0/8.0   methodology. It provides farmers with a simplified tool to calculate daily irrigation needs without needing complex desktop software.


Problem Statement
Traditional irrigation often leads to water wastage or crop stress due to a lack of precise data. This application solves that by providing a portable, web-based calculator that uses farm-level soil and crop data to determine exact water requirements.

Methodology & Formulas
The application engine is built on the   FAO Penman-Monteith   logic:

1. Crop Water Requirement ($ET_c$):  
   $$ET_c = ET_o \times K_c$$
    Where $ET_o$ is the Reference Evapotranspiration and $K_c$ is the Crop Coefficient. 

2. Volume Calculation:  
   $$\text{Total Liters} = (\text{Area in Ha} \times 10,000) \times ET_c$$
    This converts the depth of water (mm) into actual volume (Liters) for the total farm area. 



Application Logic Flowchart
The following diagram illustrates the algorithm's step-by-step execution:

 Features
- Simplified Inputs: Requires only Crop Name, Farm Area, and Soil Type.
- Smart Soil Advice: Provides management tips based on soil infiltration rates (Sandy, Loamy, or Clay).
- Responsive Design:   Works on mobile devices, tablets, and desktops.
- Instant Results:   Real-time calculation using JavaScript.

Deployment Instructions
Since this is a client-side application, it can be deployed for free:
1. Upload `index.html` to a GitHub Repository.
2. Go to   Settings > Pages  .
3. Select the   main   branch and click   Save  .
4. Your application will be live at: `https://your-username.github.io/agri-water-flow/`

Documentation & References
-   FAO Irrigation and Drainage Paper No. 56:   For $ET_o$ calculation standards.
-   CropWAT 7.0/8.0:   Software logic replication.

 Developed as a modern solution for sustainable agricultural water management. 
