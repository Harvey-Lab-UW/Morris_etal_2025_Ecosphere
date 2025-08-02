# Morris_etal_2025_Ecosphere
Data accompanying the manuscript 'Structural legacies drive variability in post-fire aboveground carbon and fuel profiles in wet temperate forests' by Morris, Laughlin, Rangel-Parra, Donato, Halofsky, Butman, and Harvey published in Ecosphere. 
*See the main text of the manuscript for complete descriptions of data collection and processing.*

[!!placeholder for Zenodo DOI badge]
[![CC BY 4.0][cc-by-shield]][cc-by]

This information is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). Any user of these data ("User" hereafter) is required to cite it appropriately in any publication that results from its use. These data may be actively used by others for ongoing research, so coordination may be necessary to prevent duplicate publication. The User is urged to contact the authors of these data for questions about methodology or results. The User is encouraged to consider collaboration or co-authorship with authors where appropriate. Misinterpretation of data may occur if used out of context of the original study. Substantial efforts are made to ensure accuracy of the data and documentation, however complete accuracy of data sets cannot be guaranteed. All data are made available as is. Data may be updated periodically and it is the responsibility of the User to check for new versions of the data. The authors and the repository where these data were obtained shall not be liable for damages resulting from any use or misinterpretation of the data.

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

---

For reproducibility, the following data files are made available: 

#### plot_info.csv

This file contains metadata associated with each sampled plot (*N* = 95). The following columns are included:

- **plot_id**: unique plot identifier in the format *site_#*
- **site**: site code indicating sampled fire
  - *bigh* = Big Hollow
  - *eagl* = Eagle Creek
  - *lion* = Lionshead
  - *nor* = Norse Peak
  - *rivr* = Riverside
- **fire_year**: calendar year of fire occurrence (YYYY)
- **sample_date**: calendar date of field data collection (YYYYMMDD)
- **easting_m**: easting coordinate of plot center, measured using a handheld Garmin GPS unit (m; projection = UTM NAD83 Zone 10N) *** SHOULD WE SHARE THESE COORDINATES?
- **northing_m**: northing coordinate of plot center, measured using a handheld Garmin GPS unit (m; projection = UTM NAD83 Zone 10N) *** SHOULD WE SHARE THESE COORDINATES?
- **slope_deg**: topographic slope at plot center, measured using a TruPulse 200 laser rangefinder (degrees)
- **aspect_deg**: topographic aspect at plot center, measured using a compass (degrees)
- **elevation_m**: elevation at plot center, measured using a handheld Garmin GPS unit (m)
- **stand_age**: categorical pre-fire stand age class, based on developmental stage as a function of community structure attributes described by [Van Pelt (2007)](https://dnr.wa.gov/sites/default/files/2025-03/lm_hcp_west_oldgrowth_guide_full_lowres.pdf)
  - *young* = ~30-50 years, established after clearcut harvest in late 1900s (Van Pelt stage = canopy closure)
  - *mid-seral* = ~70-150 years, originated from fire or clearcut harvest after Euro-American settlement (Van Pelt stages = biomass accumulation / competitive exclusion, maturation I)
  - *late-seral* = ~160-500+ years, originated from fire prior to Euro-American settlement (Van Pelt stages = maturation II, vertical diversification, horizontal diversification)
- **burn_sev**: categorical burn severity class, based on percent of overstory basal area killed by fire
  - *unburned* = 0% mortality, no signs of recent fire
  - *low* = <30% mortality
  - *high* = ≥90% mortality, stand-replacing
- **tape_length_m**: length of cardinal transect tapes, defining total plot radius and coarse woody debris transects (m)
- **tree_radius_m**: radius of tree subplots, located along each cardinal transect (m)
- **sapl_radius**: radius of sapling subplots, located along each cardinal transect (m)
- **n_slope_deg**: topographic slope of north transect tape, measured from plot center (degrees)
- **e_slope_deg**: topographic slope of east transect tape, measured from plot center (degrees)
- **s_slope_deg**: topographic slope of south transect tape, measured from plot center (degrees)
- **w_slope_deg**: topographic slope of west transect tape, measured from plot center (degrees)
- **lrgt_mult_ha**: plot-level multiplier for scaling up measurements of large trees (dbh ≥ 100 cm) to per-hectare values  *** DO WE WANT TO SHARE THESE PER-HA MULTIPLIERS? AND/OR THE SAMPLING RADII FOR TREES & SAPS?
- **tree_mult_ha**: plot-level multiplier for scaling up measurements of trees (10 ≤ dbh < 100 cm) to per-hectare values 
- **sapl_mult_ha**: plot-level multiplier for scaling up measurements of saplings (height ≥ 0.3 m, dbh < 10 cm) to per-hectare values 
- **est_seed_mult_ha**: plot-level multiplier for scaling up measurements of established seedlings (0.1 ≤ height < 0.3 m) to per-hectare values 
- **sml_seed_mult_ha**: plot-level multiplier for scaling up measurements of small seedlings (height < 0.1 m) to per-hectare values  
- **shrub_mult_ha**: plot-level multiplier for scaling up measurements of woody shrubs to per-hectare values 
- **herb_mult_ha**: plot-level multiplier for scaling up measurements of herbaceous vegetation to per-hectare values 


#### stand_structure.csv

This file contains stand-level ... description. The following columns are included:

- **col1**: description
- **col2**: description
- **col3**: description
- **basal area total**: description
- **basal area live**: description
- **basal area dead**: description
- **overstory density total**: description
- **overstory density live**: description
- **overstory density dead**: description
- **understory density total**: description
- **understory density live**: description
- **understory density dead**: description
- **live seedling density**: description
- **qmd total**: description
- **qmd live**: description
- **qmd dead**: description


#### species_composition.csv

This file contains stand-level ... description. The following columns are included:

- **col1**: description
- **col2**: description
- **col3**: description


#### biomass_carbon.csv

This file contains stand-level post-fire aboveground biomass carbon components for each sampled plot. The following columns are included:

- **col1**: description
- **col2**: description
- **col3**: description
- **total C**: description
- **live C**: description
- **dead C**: description
- **woody C**: description
- **non-woody C**: description
- **charred C**: description
- **down C (dwd)**: description
- **tree C total**: description
- **tree C live**: description
- **tree C snag**: description
- **stem wood C total (trees + cwd)**: description
- **stem wood C live**: description
- **stem wood C dead**: description
- **stem bark C total (trees + cwd)**: description
- **stem bark C live**: description
- **stem bark C dead**: description
- **stump C**: description
- **live understory C**: description



#### surface_fuels.csv

This file contains stand-level post-fire surface fuel profiles for each sampled plot. These data include down woody debris (height < 2 m), live understory vegetation, and live small saplings and seedlings (height < 1.37 m). The following columns are included:

- **col1**: description
- **col2**: description
- **col3**: description
- **fwd**: description
- **1h**: description
- **10h**: description
- **100h**: description
- **cwd**: description
- **sound**: description
- **rotten**: description
- **dwd**: description
- **deadfueldepth**: description
- **duff**: description
- **litter**: description
- **livesurface_total**: description
- **shrubs**: description
- **livesurface_woody**: description; includes woody shrubs, tree saplings / seedlings
- **livesurface_herbaceous**: description
- **live_regen**: description
- **conifer_regen**: description
- **broadleaf_regen**: description



#### canopy_fuels.csv

This file contains stand-level post-fire canopy fuel profiles for each sampled plot. These data include all live and dead canopy trees (height ≥ 1.37 m). The following columns are included:

- **col1**: description
- **col2**: description
- **col3**: description
- **foliage_total**: description
- **foliage_live**: description
- **foliage_dead**: description
- **branch_total**: description
- **branch_live**: description
- **branch_dead**: description
- **branch_1h_total**: description
- **branch_1h_live**: description
- **branch_1h_dead**: description
- **branch_10h_total**: description
- **branch_10h_live**: description
- **branch_10h_dead**: description
- **branch_100h_total**: description
- **branch_100h_live**: description
- **branch_100h_dead**: description
- **branch_1000h_live**: description
- **crown_total**: description
- **crown_live**: description
- **crown_dead**: description
- **acfl_total**: description
- **acfl_live**: description
- **acfl_dead**: description
- **cbd**: description
- **cbh**: description

