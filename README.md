# ENVS_399_PINE_BEETLES

## Problem Discription and Framing
Mountain Pine Beetle outbreaks have been prevalent for more than 30 years in the Rocky Mountains but the increasingly temperate winters in this area have led to these beetles killing tens of millions of acres of pine trees. Though outbreak severity fluctuates with droughts and heavy precipitation, predicted pine beetle spread is expected to increase quickly in the next few years leading to higher wildfire risk among other environmental issues. This is a serious cause for concern among many parties as the implications of Mountain Pine Beetle spread will affect millions of people. 

Efforts to reduce beetle kill are shown to be both possible and effective, but a large-scale project will involve lots of resources and strict coordination in order to reduce the pine beetle population in the Rockies. We look to use historical data recording Mountain Pine Beetle outbreaks in order to better predict how they’ll spread in the coming years. We’ll also use data reflecting current beetle outbreaks to devise a strategy in order to greatly decrease the beetle population.

## Repository Structure
This respository is split up into 4 folders. 
- Datasets includes all of the data that was used throughout the project. 
- Spatial Analysis contains all of the files that were used for the spatial mapping and GIS portions of the project 
- Supplementary Materials includes documents such as our annotated works cited, peer reviews and white paper draft
- Visuals contains all non spatial r code and figures. Knitted versions of the rmd files are included to not have to download the adqequate files in order to run the code.

## Datasets
1. **National Insect and Disease Detection Survey**
    - The dataset titled "National Insect and Disease Detection Survey" is an ongoing survey published and maintained by the United States Forest Service (USFS). As of 2008 when the Cooperative Forestry Assistance Act of 1978 was amended to enable the USFS to conduct surveys to appraise insect infestations they have been publishing yearly detection surveys. The downloadable geopackage files for each of the 8 regions in the US give a spatial overview of insect infestations over the years as well as some severity indicies and survey information.
    - **Some Key Variables**
        - *HOST* (discrete) - Type of tree species infected.
        - *PERCENT_AFFECTED* (continuous) - Percent of tree canopy within the polygon that are damaged or recently dead.
        - *SURVEY_YEAR* (numeric) - Year the survey was done in that paticular area.
        - *ACRES* (continuous) - Area of affected trees.
    - **Link to Dataset:** - https://www.fs.usda.gov/science-technology/data-tools-products/fhp-mapping-reporting/detection-surveys
2. **PRISM DATA**
    - The dataset titled "PRISM Weather Data" is a gathering of weather observations from a wide range of monitoring networks, assembled by a team at Oregon State University. The result is a spatial dataset published across multiple spatial and temporal resolutions that covers 1895 to present. The is free to the public project enables users to gather as much as 45 years of daily weather data, and over 100 years of monthly/yearly data.
        - **Some Key Variables:**
        - *tmean* (continuous) - Mean average temperature per year
        - *tmax* (continuous) - Maximum average temperature per year
        - *tmin* (continuous) - Minimum average temperature per year
        - *tdmean* (continuous) - Mean average dew point temperature per year
        - *ppt* (continuous) - Average amount of precipitation per year
        - *vpdmin* (continuous) - Minimum average vapor pressure index reading per year
        - *vpdmax* (continuous) - Maximum average vapor pressure index reading per year
    - **Link to Dataset** - https://prism.oregonstate.edu/
3. **Two Datasets of mountain pine beetle outbreak dynamics and direct control in Cypress Hills, SK**
    - The datasets titled "Dataset of mountain pine beetle outbreak dynamics and direct control in Cypress Hills, SK" published on Feb 26, 2020 by Kunegel-Lion, Mélodie1 et. al. details two datasets that span two different grids of cells (both of which on Saskatchewan Forest Service land), dataset one consisting of 18,317 100 × 100 m cells and dataset two being a grid of 722 500 × 500 m cells. These datasets report topological data, weather data as well as the presence of pinebeetle mitagtion among the cells between the years of 2006 and 2018. Datasets one and two share the same variables, as such the key variables are listed for both datasets.
    - **Some Key Variables:**
        - *MPB* (numeric) - Presence or number of living mountain pine beetles, eggs or larvae. 
        - *Latitude/Longitude* (continuous) - 2 variables denoting the location of each cell by latitude and longitude 
        - *Tmax* (continous) - Highest maximum daily temperature during July and August 
        - *Tmin_Summer/Tmin_Winter* (continuous) - Lowest daily temperature during July and August for the summer column and the same for winter for the winter column. 
        - *ColdTolerance* (continous) - Estimated probablity of larva survival over the winter based on temperature. 
        - *RelativeHumidity* (continuous) - Average relative humidity from march to may. 
        - *PineCover* (continous) - percentage of coverage meassuring whitebark pine, jack pine, lodgepole pine, and shore pine. 
        - *PineHeight* (continuous) - Average height of the cell's dominant tree species. 
        - *PineAge* (numeric) - Average age of the cell's dominant tree species. 
        - *BP1* (numeric) - for dataset 1: Number of infested cells, for dataset 2: or number of infested trees in a 1-cell radius from the focus cell. BP0, BP2 and BP3 have different cell radii spanning from 1 to 3. 
        - *BP1red* (numeric) - for dataset 1: Number of infested cells, for dataset 2: or number of infested trees with uncontrolled trees in a 1-cell radius from the focus cell. BP0, BP2 and BP3 have different cell radii spanning from 1 to 3. 
        - *BP1man* (numeric) - for dataset 1: Number of infested cells, for dataset 2: or number of infested trees with all trees controlled in a 1-cell radius from the focus cell. BP0, BP2 and BP3 have different cell radii spanning from 1 to 3. 
    - **Link to Datasets:** https://datadryad.org/dataset/doi:10.5061/dryad.70rxwdbt9#methods
  
## Example Figure


## Author Contributions
**Owyn** 

**Oscar** 

**Conor** 

**Sam** 

