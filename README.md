# AirQ_assessment

This project was developed for BlueSky Analytics

I measured the changes in the Air Quality in Barcelona, Spain using TROPOMI data from the satellite Sentinel-5P in the Google Earth Engine cloud computing platform. The periods of analysis was from March 16th to April 4th for 2019 and 2020, taking into account the confinement periods described in Querol et al. (2021).
For extracting the Nitrogen Dioxide (NO2) I developed a script in GEE in which the user can select two dates for data filtering, after clicking the 'Run' button the script shows the mean mosaic for the range of dates and time series of NO2 concentrations in millimol per square cm [mmol/cm^2].
The analysis phase was carried on an excel espreadsheet in which I performed the hypothesis tests on variances and medians where we can find a significant difference between both years beign the NO2 mean concentration higher than for 2020. 

Link to the script: https://code.earthengine.google.com/5e33f2a675e8cc2586b0d028c451c93f?fbclid=IwAR1RMCO1Fow8Zs9S5C2LLHeMix1cSMcCrDXFILh3n1xixErxCMKiv9UzKy0


# Methodology considerations
During the project definition and the processing step I could get some useful conclusions such as:
- There are not linear correlation between cloud fraction and NO2 concentrations (total and tropospheric).
- As the study was performed over a European city, it is important to mention that the period from March to August show low NO2 concentration values for both years because there is no need to use gas-fueled heaters at offices and houses.
- The NO2 concentrations falls every weekend but this conclusion should be studied in depth in the future.


# Future 
- The script could be converted to a GEE app with few changes, basically creating a user interface and placing the widgets.

# Reference: 
https://doi.org/10.1016/j.scitotenv.2021.146380
Querol, X., Massagué, J., Alastuey, A., Moreno, T., Gangoiti, G., Mantilla, E., … Cornide, M. J. (2021). Lessons from the COVID-19 air pollution decrease in Spain: Now what? Science of The Total Environment, 779, 146380. doi:10.1016/j.scitotenv.2021.146380 
