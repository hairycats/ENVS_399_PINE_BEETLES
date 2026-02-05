# ENVS_399_PINE_BEETLES

## Problem Discription and Framing
Mountain Pine Beetle outbreaks have been prevalent for more than 30 years in the Rocky Mountains but the increasingly temperate winters in this area have led to these beetles killing tens of millions of acres of pine trees. Though outbreak severity fluctuates with droughts and heavy precipitation, predicted pine beetle spread is expected to increase quickly in the next few years leading to higher wildfire risk among other environmental issues. This is a serious cause for concern among many parties as the implications of Mountain Pine Beetle spread will affect millions of people. 

Efforts to reduce beetle kill are shown to be both possible and effective, but a large-scale project will involve lots of resources and strict coordination in order to reduce the pine beetle population in the Rockies. We look to use historical data recording Mountain Pine Beetle outbreaks in order to better predict how they’ll spread in the coming years. We’ll also use data reflecting current beetle outbreaks to devise a strategy in order to greatly decrease the beetle population.

## Datasets
1. **Reconstructing historical outbreaks of mountain pine beetle in lodgepole pine forests in the Colorado Front Range**
   - The data set “Reconstructing historical outbreaks of mountain pine beetle in lodgepole pine forests in the Colorado Front Range” by Jose F. Negron is a data set composed of data on trees found that were killed by pine beetles in Colorado, which were collected during the summers of  2012, 2013, and 2015.
   - **Some Key Variables:**
     - *Site* (Nominal) - the site name
     - *estab_date* (oridnal) - the year of the tree’s establishment
     - *death_date* (ordinal) - the year it is expected that the tree died
     - *age* (numeric) - the age of the tree at the time of death
     - *dbh_cm* (continous) - the tree’s diameter at breast height in centimeters
    - **Link to Dataset:** https://www.fs.usda.gov/rds/archive/catalog/RDS-2020-0036
2. **Mountain pine beetle attack severity data in lodgepole pine in the Northern Rockies from 1999-2014**
   - Published in 2018, the dataset “Mountain pine beetle attack severity data in lodgepole pine in the Northern Rockies from 1999-2014” by Howard L. Williams, Sharon M. Hood, Christopher R. Keyes, and Joel M. Egan includes data on the severity and spread of mountain pine beetles and their impact on lodgepole pine species across the many subwatersheds in parts of Washington, Idaho, Montana, and Wyoming. This dataset pulls from the USDA Forest Service’s Aerial Insect and Disease Detection Survey.
This dataset is a file geodatabase, which contains spatial data used for GIS. So in this dataset, we have spatial features, each of which has attribute information.
    - **Some Key Variables:**
      - *OBJECTID* (ordinal) - a unique identification number for each subwatershed
      - *HUC_Acres* (continuous) - total area of the subwatershed in acres
      - *lpp1* (continuous) - acres of lodgepole pine not attacked by MPB (in the given subwatershed)
      - *lpp2* (continuous) - acres of lodgepole pine acres attacked by MPB (in the given subwatershed)
      - *tpa1* (continuous) - mean number of lodgepole pine trees per acre not attacked by MPB
      - *tpa2* (continuous) - mean number of lodgepole pine trees per acre attacked by MPB
      - *sdi1* (continuous) - mean stand density index, or how densely the trees are clustered, per acre for lodgepole pine not attacked by MPB.
      - *sdi2* (continuous) - mean stand density index, or how densely the trees are clustered, per acre for lodgepole pine attacked by MPB.
    - **Link to Dataset:** https://www.fs.usda.gov/rds/archive/catalog/RDS-2017-0006
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

