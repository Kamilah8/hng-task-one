# OUTLIER DETECTION ELECTION REPORT 
 
## Case Study
Ensuring Election Integrity in the recently concluded election. The Independent National Electoral Commission(INEC) has faced multiple legal challenges concerning the integrity and accuracy of the election results. Allegations of vote manipulation and irregularities have been widespread, prompting a thorough investigation into the matter.


 
## INTRODUCTION
This report investigates the integrity and accuracy of the recently concluded election overseen by the Independent National Electoral Commission (INEC) in Oyo State. Given multiple legal challenges and allegations of vote manipulation, I conducted a thorough analysis to identify outlier polling units with significant deviations in voting results compared to neighboring units. In the recent election, INEC faced allegations of vote manipulation and irregularities, prompting an investigation into the accuracy of the reported results. This report outlines our methodology, findings, and recommendations for identifying and addressing potential voting irregularities.
**Project Purpose**
This analysis aims to ensure transparency and uphold the democratic process.
 
METHODOLOGY
1.    Selection of data and extraction using Geographical Location: Latitude and Longitude details for each polling unit of Oyo state was extracted, using the Geocoding on Google Sheet.
2.    Data Cleaning: Removed duplicate by using the Data cleanup option on Google Sheet and the data filtering option to visually inspect and VLOOKUP to manage errors and missing data cells. This is to ensure a complete and accurate dataset.
3.    Using Google Sheets For Geospatial Analysis: This is the examination of data that is tied to a specific location. Geospatial analysis was used to identify the neighboring polling unit in OYO State based on the geographical proximity.
 
 The Haversine Formular was used to calculate the distance between each pair of polling units based on their Latitude and Longitude with a proximity radius of 1km. 
 Where Latitude and Longitude was converted to Radians using this formula   ``Radians(C2)``

The Harversine Formula is used for calculating distances between two points on a sphere(earth).
``d=2r * sin2 (SQRT(SIN2(Δφ/2​) + cos(φ1​) ⋅ cos(φ2​) ⋅ sin2(Δλ/2​)``


 
where:
*  ``φ1\varphi_1φ1​ and φ2\varphi_2φ2​`` are the latitudes of the two points (in radians).
*  ``λ1\lambda_1λ1​ and λ2\lambda_2λ2​`` are the longitudes of the two points (in radians).
*  ``Δφ=φ2−φ1\Delta \varphi = \varphi_2 - \varphi_1Δφ=φ2​−φ1​``is the difference in latitude.
*  ``Δλ=λ2−λ1\Delta \lambda = \lambda_2 - \lambda_1Δλ=λ2​−λ1``​ is the difference in longitude.
R is the Earth's radius (mean radius = 6,371 km).
d is the distance between the two points.
 
### Outlier
An outlier is a data point that significantly differs from other observations in a dataset. It can indicate variability in the data, errors, or unique phenomena. Detecting outliers is essential in many fields to ensure data integrity and accurate analysis.
The statistical methods such as Average and standard deviation to detect outliers of each polling unit.

**Formula**

``Z= (X−μ) σ ``​
where X is the data point, μ is the mean, and σ is the standard deviation.
 


### Findings 
##### Top 3- Outliers for APC

**PU-NAME**                                **Outliers**
PRIMARY SCHOOL, IDI ORO ELEWA             7.2922736
I.D.C. PRIMARY SCHOOL, AWOTAN             6.620963928

OLUWO VILLAGE
5.844793814

 
Top 3- Outliers for LP
ST. JAMES AFRICAN CHURCH,ISOPAKO
15.07253538
COMMUNITY PRIMARY SCHOOL,KARAMO
13.08053282
QUEEN’S HALL, U.I
12.45926055

 
Top 3- Outliers for PDP
WAKAJAYE PRIMARY SCHOOL
2.787418369
I.D.C. PRIMARY SCHOOL, OPE ODU
2.246140793
HEALTH CLINIC, TEGE
2.038446772

 




Top 3- Outliers for NNPP
OPEN SPACE OLORISA OKO JUNCTION OPPOSITE A TRANSFORMER
1794.404637
COMMUNITY PRIMARY SCHOOL, TESI APATA
660.4071574
ARMY BARRACKS I
610.8621645

 
Over all Top 3- Outliers
OPEN SPACE OLORISA OKO JUNCTION OPPOSITE TRANSFORMER
1794.404637
ST. JAMES AFRICAN CHURCH, ISOPAKO
15.07253538
PRIMARY SCHOOL, IDI ORO ELEWA
7.2922736

 
 
 
 
 
 A correlation between LP and PDP




### CONCLUSION
The geospatial analysis and outlier detection identified a deviation in voting patterns for the APC and LP parties with NNPP having a high outlier.
Outliers in NNPP data suggest pontiac areas for further investigation.
 
 


