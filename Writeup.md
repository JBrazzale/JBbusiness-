## Pitching a Clustering Model to BetterHelp (Joseph Brazzale)


### Abstract
The main goal of this project is to determine the optimal areas in the United States to target with ads for a telehealth therapy company. 
This preliminary analysis can then be used to build a sophisticated clustering model to determine which people are at the highest risk 
of self-harm. Remote care provides a great opportunity to provide therapy to underserved areas in the US. As this is an emerging technology 
in the healthcare space, gaining a solid subscriber base is key to this business's success. Additionally, this can help reduce the number 
of self-harm cases.

### Design
For this project, I wanted to build a few simple visualizations that can illustrate that there are in fact areas with greater needs. 
I requested the mortality data from the National Vital Statistics System which is a division of the CDC. This database contains all of the deaths 
from suicide by county from the years 2008-20014. I also pulled the data from the NCHS, which classifies which counties are urban, and which ones are rural.
Finally, I pulled all of the locations of hospitals and clinics from the AHA.

### Data
My initial request from the NVSS returned a database with over 3200 data points. There were some counties that had missing values
for deaths, these were removed. The geographical data in this file was split into two columns, I concatenated them into a single
FIPS code, which uniquely identifies areas. Areas with higher populations had an overall greater number of deaths, so I added a
deaths per 100,000 to see which states had the highest rates. Finally, I set a filter on my hospital data to remove all of the medical
facilities that were not psychiatric facilities.

### Algorithms
- Rate for all deaths was adjusted to the death rate per 100,000


### Tools
- Initial data cleaning was performed in DB Browser for SQLite
- Further data exploration was done in Microsoft Excel
- All visualizations were made using Tableau

### Communication
This project will be presented to the client using a PowerPoint presentation. This presentation will function as proof of
concept for my model. 
