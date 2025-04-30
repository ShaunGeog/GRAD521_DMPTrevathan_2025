# GRAD521_DMPTrevathan_2025

Data Management Plan for the research project Storm Surge Risk: A Spatial Analysis of Volusia County's At-Risk Communities

Date: 04/30/2025
Author: Shaun Trevathan


Context of the project:

The aim for this project is to answer the following research question: Which areas within Volusia County, Florida have the highest concentrations of vulnerable populations to storm surge, and how do factors such as geography, income, age, and prevalence of chronic disease contribute to this vulnerability?  This is important because coastal flooding events have been increasing in intensity and frequency since 1950 along both the Gulf of Mexico and the coast of the Atlantic Ocean (EPA, 2022).  A 2020 study investigated 21 hurricanes and their associated storm surge between the years of 2000 and 2013 and found that the volume for storm surge in 14 storms increased by 36% and the extent of inundation increased by 25% for 13 of the storms (Camelo, Mayo, & Gutmann, 2020).  Camelo et al, found that of the states that were at the most risk for these events was the state of Florida amongst others (2020).




Data Description:

To answer the research question, I will be using spatial datasets and ArcGIS Pro software to map the various social and geographic variables and conduct a weighted overlay analysis based on weights that will be determined using an analytical hierarchy process (AHP). The results of the analysis will show where areas of highest to lowest vulnerability are located across the county. For the analysis I will be using nine different variables (two physical variables, storm surge depth and area) and seven social variables which are based on common vulnerability criteria (percent of individual 65 years old and older, percent of people under 18 years of age, income, prevalence of COPD, coronary heart disease, stroke, and diabetes).
  
To map the storm surge variables, I will be using two separate datasets.  One data set is a digital elevation model (DEM) that will be acquired from the United States Geological Survey (USGS).  It will consist of four raster tiles.  The tiles will be in different file sizes due to the amount of elevation data visible in each image. The file sizes are 20.0MB, 53.3MB, 1.25MB, and 49.7MB.  These tiles will be combined in ArcGIS Pro and then clipped to a shapefile of the Volusia County boundary (133KB) so that there will be no extraneous data, as I only want the elevation data for the county. The DEM will be used in the analysis to determine the role that storm surge depth will have on the different vulnerable populations. The final dataset for the physical variables is a polygon shapefile that maps the area or extent of storm surge inundation as it relates to a category 1-5 hurricane (579MB).
  
For the social variables I will be using data provided by the United States Census at both the Census Tract and Census Block Group levels.  This data will be used to identify where the individuals who are 65 years old and older and those who are under 18 years old are located across the county.  Both age ranges are identified as being at greatest risk to hazard events.  Additionally, the variable for income will be taken from the census data as well.  The size of the U.S. Census dataset is 991MB.

The last remaining dataset that I will be using is the Center for Disease Control’s PLACES: Local Data for Better Health, which is at the Census Tract level to avoid patient identification.  This dataset will provide the percentage of prevalence for the four chronic diseases I will be including in my risk assessment, as these diseases present the most complications for individuals during a hazard event.  The size of this dataset is 4.09GB.  These are the sizes of the datasets as they were obtained, and they will likely change in size as the data will be isolated to the boundaries of the county, as some of this data includes data from other counties, and in the case of the PLACES dataset includes disease prevalence data from across the nation.

None of the data that I will be using will be collected or created by me.  This data is provided by federal agencies (U.S. Census data, USGS, and the PLACES: Local Data for Better Health) or from the Volusia County, Florida GIS Data Portal (county boundary and storm surge inundation shapefiles).  Except for the U.S. Census data, all of the datasets are in the form of shapefiles or as a raster file (DEM).  Shapefiles are a file format that is used in spatial analysis, as are raster datasets.  The U.S. Census data is provided in two different data types, as a shapefile, which consists of georeferenced boundaries (Census Tracts, Block Groups, or Blocks) and a csv file that contains the actual census data.  To map the census data the csv file must be joined to the boundary shapefile, which is done within ArcGIS Pro or other spatial analysis software. 



Roles and Responsibilities:

I am the sole member of the research team.  All of the data management, data acquisition, data preservation, and data analysis will be performed by myself without any assistance from my committee chair, outside of an advisory role if I have any questions.  All of my data comes from federal and local governmental GIS data portals, and the project does not require any in-situ data collection, so there is no need for instrumentation maintenance or calibration.  All metadata creation has already been created by the data creators.  Quality control will be handled by myself as I verify that there are no missing values in the data, or that there are no data points that have been geocoded improperly.  For this project, as there are no associated funding sources, nor is it required for the capstone requirements, there will be no generation of a data management plan. As I am the only member of the research team, and not under the employment of another individual or organization, there is no need for a contingency plan. 




Data Standards and metadata:

There are no formal data management requirements concerning my research data.  I have not been informed by my department or committee chair of any departmental or institutional concerns that must be accounted for.  There are also no regulations concerning privacy issues surrounding my data, as privacy measures were already accounted for in the creation of the data by the federal agencies.  The data sets that are being used in this project include spatial data on physical geography features or flooding inundation, which has not privacy concerns attached to it.  The remaining data consists of United States Census data, which does not provide any details that can be attached to an individual, the same applies to the CDC data set (PLACES: Local Data for Better Health) as the disease prevalence data is at the Census Tract level, which is at too large of a scale to be able to identify where individuals with chronic illnesses live.




Storage and security:

The data will be stored on my personal computer as well as on a series of external hard drives that only I have access to.




Access and data sharing:

The data and the associated spatial analysis project folders will be stored on the hard drive of my laptop, which is where the spatial analysis will be conducted, and on three external solid state hard drives.  There is one primary external hard drive that the analyses will be performed from, to prevent any loss of data or completed analyses if the laptop has any malfunctions.  As analyses are completed, or iterations of analyses that are completed, from the primary external hard drive, copies of the updated project folder are saved to the laptop’s hard drive and the remaining two other external hard drives. No software packages are used in this process outside of the project folder, and its associated geodatabase, that is created by the spatial analysis software, Esri’s ArcGIS Pro.  As there are no other members of the research team, there data is not saved to a shared drive.  The project data folder, and its associated data folder where the data sets are stored, are not currently stored in a cloud-based system.  I have not tried compressing the files as a zipped folder and uploading to a DropBox or a similar platform.  I have not considered this option since I have four copies saved.  If I do decide to use a cloud-based system I will see if I can upload the data to a personal cloud storage, so that the data is not lost once I graduate from OSU.



References:

Camelo, J., Mayo, T. L., & Gutmann, E. D. (2020). Projected climate change impacts on hurricane storm surge inundation in the coastal United States. Frontiers in Built Environment, 6. https://doi.org/10.3389/fbuil.2020.588049.
 
U.S. Environmental Protection Agency. (2022). Climate Change Indicators: Coastal Flooding. Retrieved from https://www.epa.gov/climate-indicators/climate-change-indicators-coastal-flooding 



