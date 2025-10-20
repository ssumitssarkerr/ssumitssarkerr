# Save this as create_cv.py and run with Python 3

import os

cv_content = """
# Sumit Sarker
**Oceanography Graduate | Research Assistant | Marine & Environmental Scientist**

📍 Sonapur Road, Noakhali 3814, Bangladesh
📞 +8801629015976
📧 ssumitssarkerr@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/sumitsarker/
🔗 ResearchGate: https://www.researchgate.net/profile/Sumit-Sarker

---

## Education

| Exam | Institution / Board | GPA / CGPA | Year |
|------|-------------------|------------|------|
| B.Sc. in Oceanography | Noakhali Science and Technology University (NSTU), Bangladesh | CGPA: 3.81/4.00 | 2020–2025 |
| Higher Secondary Certificate (HSC) | Government City College, Chattogram, Bangladesh | GPA: 5.00/5.00 | 2017–2019 |
| Secondary School Certificate (SSC) | Nasirabad Government High School, Chattogram, Bangladesh | GPA: 5.00/5.00 | 2012–2017 |

---

## Research Experience
**Research Assistant** – NOAMI, Bangladesh (2021–Present)
- Flood Susceptibility Mapping & Hydraulic Modeling
- Multi-Hazard Coastal Vulnerability Assessment
- Microplastics in Estuarine Plankton
- Bioaccumulation of Microplastics
- Flood Impact Study (Aug 2024)

---

## Academic Project
**Detection and Analysis of Marine Heatwaves in the Bay of Bengal: ENSO, IOD, and Chlorophyll Dynamics**
- Monitored SST anomalies (1982–2025)
- Assessed MHW frequency, intensity, duration
- Investigated correlations between MHW and chlorophyll-a
- Proposed adaptive strategies for ecosystem resilience

---

## Posters & Presentations
1. Integration of Multi-Criteria Decision Analysis and GIS for Aquaculture Site Suitability
   [ResearchGate Link](https://www.researchgate.net/publication/396454659_Integration_of_Multi-Criteria_Decision_Analysis_MCDA_and_GIS_for_Aquaculture_Site_Suitability_in_Hatiya_Upazila_Noakhali_Bangladesh)
2. Enhancing Aquaculture Water Quality Using Water Hyacinth
   [ResearchGate Link](https://www.researchgate.net/publication/395932974_Enhancing_Aquaculture_Water_Quality_Using_Water_Hyacinth_in_Ponds)
3. Flood Susceptibility Mapping in Noakhali, Bangladesh
   [ResearchGate Link](https://www.researchgate.net/publication/395927596_Flood_Susceptibility_Mapping_in_Noakhali_Bangladesh_Using_GIS-Based_Multi-Criteria_Decision_Analysis_MCDA_and_the_Analytical_Hierarchy_Process_AHP)
4. Phytoplankton Responses to Extreme Weather
5. Coastal Erosion and Accretion Analysis
6. Evaluating Plankton Dynamics in Salt Marshes
7. Impact of Fertilizers on Plankton & Shrimp Growth
   [ResearchGate Link](https://www.researchgate.net/publication/395956733_Evaluating_the_Impact_of_Diverse_Fertilizers_on_Plankton_Abundance_and_Shrimp_Growth_Rates_in_Aquaculture)
8. Geospatial Analysis of Coastal Erosion & Sediment Accretion
   [ResearchGate Link](https://www.researchgate.net/publication/395959134_Geospatial_Analysis_of_Coastal_Erosion_and_Sediment_Accretion_in_Southern_Hatiya_Island_Bangladesh)

---

## Writing & Proposal Experience
- NOAMI Ocean Olympiad 2024 – 1st Prize
- NOAMI Ocean Olympiad 2025 – Joint Runner-up

---

## Technical Skills
**Programming:** Python, MATLAB, R, IBM SPSS  
**GIS & Remote Sensing:** ArcGIS, QGIS, Google Earth Engine  
**Modeling:** HEC-RAS, HEC-GeoRAS, Delft 3D  
**Field & Lab:** Water/soil sampling, plankton analysis, microplastic extraction  
**Graphics & Documentation:** Adobe Photoshop, Illustrator, InDesign, MS Office, Google Workspace

---

## Awards & Honors
- University Merit Scholarship (2024–2025)
- Best Poster Presenter – ICSF 2025
- Best Poster Presenter – 2nd Comilla University Science Club
- 3rd Place Poster – Electronics & Electrical Engineering Day 2024, NSTU

---

## Leadership & Involvement
- Office Intern – NSTU Ranking and Strategic Development Cell
- Executive Member – NSTU Science Club R&D Wing
- Campus Ambassador – Scholarship School BD & SOI Academy
- General Member – NSTU Research Society & Cholo Paltai Foundation

---

## Languages
- Bangla – Native  
- English – Professional

---

## References
**Md Mesbah Uddin Bhuiyan** – Assistant Professor, NSTU  
📱 +8801722362222 | ✉️ mesbah.ocn@nstu.edu.bd  

**Imtiaj Ahmed Easty** – Assistant Professor, NSTU  
📱 +8801521249748 | ✉️ imtiaj.ocn@nstu.edu.bd
"""

# Save as Markdown
with open("Sumit_Sarker_CV.md", "w", encoding="utf-8") as f:
    f.write(cv_content)

print("✅ Markdown CV created: Sumit_Sarker_CV.md")

# Optional: Convert Markdown to PDF (requires markdown2 + pdfkit)
try:
    import markdown2
    import pdfkit

    html_content = markdown2.markdown(cv_content)
    pdfkit.from_string(html_content, "Sumit_Sarker_CV.pdf")
    print("✅ PDF CV created: Sumit_Sarker_CV.pdf")
except ImportError:
    print("⚠️ Install markdown2 and pdfkit to generate PDF: pip install markdown2 pdfkit")
    print("Also, install wkhtmltopdf for pdfkit to work.")
