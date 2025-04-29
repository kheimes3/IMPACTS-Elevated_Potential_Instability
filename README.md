# IMPACTS-Elevated-Convection-Analysis
This repository contains the code used to study elevated potential instability (EPI) within wintertime extratropical cyclones that were sampled during the IMPACTS field campaign. Follow the steps below:
1) Create the files for the statistical analysis (Folder: File_Creation)
   - EPI_IdentPT1_CrossSectionCalculations: Create vertical cross sections of equivalent potential temperature w.r.t ice and water using HRRR initialization data along an aircraft track
   - EPI_IdentPT2_LayerIdent: Identify layers of EPI w.r.t water or ice
   - LowRel_PGrad_FileCreater: Transform aircraft track from Latitude/longitude coordinates to low relative coordinates and calculate cyclone pressure gradient
   - ProcessingCRSVrData: Process W-band Vr data following Lundstrom et al. 2025b
   - Vr-SaveFilesByCategories: Create files of Vr within specific layers
3) Statistical Analysis of hydrometeor vertical motions and EPI characteristics
   - EPICharacteristics: Uses EPI layer and Low Relative files to statistically analyze EPI characteristics
   - Vr-CycloneStrengthType: Creates histograms of Vr by cyclone categories
   - Vr-Stable_EPI_EPIStrength: Creates histograms of Vr by layer stability and EPI characteristics

## This code was used for the analysis in the following studies:
Lundstrom, K. H., R. M. Rauber, G. M. Heymsfield, M. W. McLinden, and L. McMurdie, 2025: Manifestation of Elevated Convection within Wintertime Extratropical Cyclones during IMPACTS: Part I: Analysis of Elevated Potential Instability. J. Atmos. Sci., https://doi.org/10.1175/JAS-D-24-0198.1, in press.

Lundstrom, K. H., R. M. Rauber, M. W. McLinden, J. A. Finlon, G. M. Heymsfield, and L. McMurdie, 2025: Manifestation of Elevated Convection within Wintertime Extratropical Cyclones during IMPACTS: Part II: Hydrometeor Vertical Motions within and outside of Elevated Potentially Unstable Layers. J. Atmos. Sci., https://doi.org/10.1175/JAS-D-24-0199.1, in press.

## Data Required:
- Winterstorms database for IMPACTS (included in repository)
- ERA5 Surface data (https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels?tab=overview)
- IMPACTS radar data (https://www.earthdata.nasa.gov/data/projects/impacts/collection)
- IMPACTS flight track data (https://www.earthdata.nasa.gov/data/projects/impacts/collection)
- HRRR initialization data (download in EPI_IdentPT1_CrossSectionCalculations.ipynb)
