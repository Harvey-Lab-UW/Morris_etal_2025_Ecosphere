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

### plot_info.csv

This file contains metadata associated with each sampled plot (*N* = 95). The following columns are included:

- **plot_id**: unique plot identifier in the format *site_plot#*
- **site**: site code indicating sampled fire
  - *bigh* = Big Hollow
  - *eagl* = Eagle Creek
  - *lion* = Lionshead
  - *nor* = Norse Peak
  - *rivr* = Riverside
- **fire_year**: calendar year of fire occurrence (YYYY)
- **sample_date**: calendar date of field data collection (YYYYMMDD)
- **slope_deg**: topographic slope at plot center (degrees), measured using a TruPulse 200 laser rangefinder
- **aspect_deg**: topographic aspect at plot center (degrees), measured using a compass
- **elevation_m**: elevation at plot center (m), measured using a handheld Garmin GPS unit
- **stand_age**: categorical pre-fire stand age class, based on developmental stage as a function of community structure attributes described by [Van Pelt (2007)](https://dnr.wa.gov/sites/default/files/2025-03/lm_hcp_west_oldgrowth_guide_full_lowres.pdf)
  - *young* = ~30–50 years, established after clearcut harvest in late 1900s (Van Pelt stage = canopy closure)
  - *mid-seral* = ~70–150 years, originated from fire or clearcut harvest after Euro-American settlement (Van Pelt stages = biomass accumulation / competitive exclusion, maturation I)
  - *late-seral* = ~160–500+ years, originated from fire prior to Euro-American settlement (Van Pelt stages = maturation II, vertical diversification, horizontal diversification)
- **burn_sev**: categorical burn severity class, based on percent of overstory basal area killed by fire
  - *unburned* = 0% mortality, no signs of recent fire
  - *low* = <30% mortality
  - *high* = ≥90% mortality, stand-replacing
- **tape_length_m**: length of cardinal transect tapes (m), defining total plot radius and coarse woody debris transects
- **tree_radius_m**: radius of tree subplots (m), located along each cardinal transect
- **sapl_radius**: radius of sapling subplots (m), located along each cardinal transect
- **n_slope_deg**: topographic slope of north transect tape (degrees), measured from plot center
- **e_slope_deg**: topographic slope of east transect tape (degrees), measured from plot center
- **s_slope_deg**: topographic slope of south transect tape (degrees), measured from plot center
- **w_slope_deg**: topographic slope of west transect tape (degrees), measured from plot center
- **lrgt_mult_ha**: plot-level multiplier for scaling up sampled large trees (dbh ≥ 100 cm) to per-hectare values 
- **tree_mult_ha**: plot-level multiplier for scaling up sampled trees (10 ≤ dbh < 100 cm) to per-hectare values 
- **sapl_mult_ha**: plot-level multiplier for scaling up sampled saplings (height ≥ 0.3 m, dbh < 10 cm) to per-hectare values 
- **est_seed_mult_ha**: plot-level multiplier for scaling up sampled established seedlings (0.1 ≤ height < 0.3 m) to per-hectare values 
- **sml_seed_mult_ha**: plot-level multiplier for scaling up sampled small seedlings (height < 0.1 m) to per-hectare values  
- **shrub_mult_ha**: plot-level multiplier for scaling up sampled woody shrubs to per-hectare values 
- **herb_mult_ha**: plot-level multiplier for scaling up sampled herbaceous vegetation to per-hectare values 



### stand_structure.csv

This file contains stand-level post-fire structure summaries for each sampled plot. The following columns are included:

- **plot_id**: unique plot identifier in the format *site_plot#*
- **basalarea_m2_ha**: basal area (m<sup>2</sup>/ha), all trees (height ≥ 1.37 m)
- **basalarea_m2_ha_live**: basal area (m<sup>2</sup>/ha), live trees (height ≥ 1.37 m)
- **basalarea_m2_ha_dead**: basal area (m<sup>2</sup>/ha), dead trees (height ≥ 1.37 m)
- **overstory_stems_ha**: stem density (stems/ha), all overstory trees (dbh ≥ 10 cm)
- **overstory_stems_ha_live**: stem density (stems/ha), live overstory trees (dbh ≥ 10 cm)
- **overstory_stems_ha_dead**: stem density (stems/ha), dead overstory trees (dbh ≥ 10 cm)
- **understory_stems_ha**: stem density (stems/ha), all understory trees (dbh < 10 cm, height ≥ 0.3 m)
- **understory_stems_ha_live**: stem density (stems/ha), live understory trees (dbh < 10 cm, height ≥ 0.3 m)
- **understory_stems_ha_dead**: stem density (stems/ha), dead understory trees (dbh < 10 cm, height ≥ 0.3 m)
- **seedling_stems_ha_live**: stem density (stems/ha), live seedlings (height < 0.3 m)
- **qmd_cm**: quadratic mean diameter (cm), all overstory trees (dbh ≥ 10 cm)
- **qmd_cm_live**: quadratic mean diameter (cm), live overstory trees (dbh ≥ 10 cm)
- **qmd_cm_dead**: quadratic mean diameter (cm), dead overstory trees (dbh ≥ 10 cm)



### species_composition.csv

This file contains stand-level post-fire species composition for each sampled plot. Composition is summarized for all trees with height ≥ 1.37 m. The following columns are included:

- **plot_id**: unique plot identifier in the format *site_plot#*
- **species**: four-letter tree species code
  - *abam* = *Abies amabilis* (Douglas ex Loudon) Douglas ex Forbes
  - *abgr* = *Abies grandis* (Douglas ex D. Don) Lindl.
  - *abla* = *Abies lasiocarpa* (Hook.) Nutt.
  - *abpr* = *Abies procera* Rehder
  - *acgl* = *Acer glabrum* Torr.
  - *acma* = *Acer macrophyllum* Pursh
  - *alru* = *Alnus rubra* Bong.
  - *cano* = *Callitropsis nootkatensis* (D. Don) Oerst. ex D.P. Little
  - *chch* = *Chrysolepis chrysophylla* (Douglas ex Hook.) Hjelmqvist
  - *conu* = *Cornus nuttallii* Audubon ex Torr. & A. Gray
  - *laoc* = *Larix occidentalis* Nutt.
  - *pico* = *Pinus contorta* Douglas ex Loudon var. *latifolia* Engelm. ex S. Watson
  - *pien* = *Picea engelmannii* Parry ex Engelm.
  - *pimo* = *Pinus monticola* Douglas ex D. Don
  - *poba* = *Populus balsamifera* L. ssp. *trichocarpa* (Torr. & A. Gray ex Hook.) Brayshaw
  - *prem* = *Prunus emarginata* (Douglas ex Hook.) D. Dietr.
  - *psme* = *Pseudotsuga menziesii* (Mirb.) Franco
  - *tabr* = *Taxus brevifolia* Nutt.
  - *thpl* = *Thuja plicata* Donn ex D. Don
  - *tshe* = *Tsuga heterophylla* (Raf.) Sarg.
  - *tsme* = *Tsuga mertensiana* (Bong.) Carrière
- **group**: functional group code describing the shade-tolerance, leaf morphology, and reproductive classification of each tree species
  - *i* = shade-intolerant conifer / gymnosperm
  - *t* = shade-tolerant conifer / gymnosperm
  - *b* = broadleaf / angiosperm
- **live_dbh_min_cm**: minimum dbh (cm), live individuals
- **dead_dbh_min_cm**: minimum dbh (cm), dead individuals
- **live_dbh_min_cm**: maximum dbh (cm), live individuals
- **dead_dbh_min_cm**: maximum dbh (cm), dead individuals
- **live_basalarea_m2_ha**: basal area (m<sup>2</sup>/ha), live individuals
- **dead_basalarea_m2_ha**: basal area (m<sup>2</sup>/ha), dead individuals
- **live_stems_ha**: density (stems/ha), live individuals
- **dead_stems_ha**: density (stems/ha), dead individuals



### biomass_carbon.csv

This file contains stand-level post-fire aboveground biomass carbon components for each sampled plot. All values are Mg C/ha. The following columns are included:

- **plot_id**: unique plot identifier in the format *site_plot#*
- **c_total_Mg_ha**: total aboveground biomass; includes all standing trees, stumps, down woody debris, and understory vegetation
- **c_live_Mg_ha**: live aboveground biomass; includes all standing live trees and understory vegetation
- **c_dead_Mg_ha**: dead aboveground biomass; includes all standing dead trees, stumps, and down woody debris
- **c_woody_Mg_ha**: woody biomass; includes branches and stems of standing trees, stumps, down woody debris, and woody shrubs
- **c_nonwoody_Mg_ha**: non-woody biomass; includes tree foliage and total mass of herbaceous understory vegetation
- **c_standing_Mg_ha**: total standing tree biomass; includes foliage, branches, and stems of all trees
- **c_standing_Mg_ha_live**: standing live tree biomass; includes foliage, branches, and stems of live trees
- **c_standing_Mg_ha_dead**: standing dead tree biomass; includes foliage, branches, and stems of dead trees
- **c_stump_Mg_ha**: total stump biomass; includes stem wood and bark of trees with broken top and height < 1.37 m
- **c_stemwood_Mg_ha**: total stem wood biomass; includes all standing trees (height ≥ 1.37 m) and coarse woody debris (1000-h particles, diameter ≥ 7.6 cm)
- **c_stemwood_Mg_ha_live**: live stem wood biomass; includes standing live trees (height ≥ 1.37 m)
- **c_stemwood_Mg_ha_dead**: dead stem wood biomass; includes standing dead trees (height ≥ 1.37 m) and coarse woody debris (1000-h particles, diameter ≥ 7.6 cm)
- **c_stembark_Mg_ha**: total stem bark biomass; includes all standing trees (height ≥ 1.37 m) and coarse woody debris (1000-h particles, diameter ≥ 7.6 cm)
- **c_stembark_Mg_ha_live**: live stem bark biomass; includes standing live trees (height ≥ 1.37 m)
- **c_stembark_Mg_ha_dead**: dead stem bark biomass; includes standing dead trees (height ≥ 1.37 m) and coarse woody debris (1000-h particles, diameter ≥ 7.6 cm)
- **c_dwd_Mg_ha**: down woody debris biomass; includes stem wood and bark of all fine (1-, 10-, 100-h particles, diameter < 7.6 cm) and coarse (1000-h particles, diameter ≥ 7.6 cm) fuel components
- **c_understory_Mg_ha**: live understory biomass; includes foliage, branches, and stems of woody shrubs, herbaceous vegetation, and tree seedlings and small saplings (height < 1.37 m)
- **c_charred_Mg_ha**: charred wood biomass; includes black carbon in charred stem wood on standing trees (height ≥ 1.37 m) and coarse woody debris (1000-h particles, diameter ≥ 7.6 cm)



### surface_fuels.csv

This file contains stand-level post-fire surface fuel profiles for each sampled plot. These data include aboveground biomass of down woody debris (height < 2 m), live understory vegetation, and live understory trees (height < 1.37 m). The following columns are included:

- **plot_id**: unique plot identifier in the format *site_plot#*
- **dwd_Mg_ha**: total down woody debris fuel load (Mg/ha); includes fine (diameter < 7.6 cm) and coarse (diameter ≥ 7.6 cm) fuels
- **fwd_Mg_ha**: total fine woody debris fuel load (Mg/ha); includes 1-h (diameter < 0.6 cm), 10-h (0.6 ≤ diameter < 2.5 cm), and 100-h (2.5 ≤ diameter < 7.6 cm) particles
- **one_hour_Mg_ha**: fuel load of 1-h fuel particles (diameter < 0.6 cm; Mg/ha)
- **ten_hour_Mg_ha**: fuel load of 10-h fuel particles (0.6 ≤ diameter < 2.5 cm; Mg/ha)
- **hundred_hour_Mg_ha**: fuel load of 100-h fuel particles (2.5 ≤ diameter < 7.6 cm; Mg/ha)
- **cwd_Mg_ha**: total coarse woody debris fuel load (Mg/ha); includes all 1000-h particles (diameter ≥ 7.6 cm)
- **cwd_Mg_ha_sound**: fuel load of sound coarse woody debris (Mg/ha); includes 1000-h particles (diameter ≥ 7.6 cm) with decay class 1–3
- **cwd_Mg_ha_rotten**: fuel load of rotten coarse woody debris (Mg/ha); includes 1000-h particles (diameter ≥ 7.6 cm) with decay class 4–5
- **deadfuel_depth_cm**: mean depth of dead fuel (cm); includes dead woody and non-woody plant material (height < 2 m)
- **duff_depth_cm**: mean depth of duff (cm)
- **litter_depth_cm**: mean depth of litter (cm)
- **live_surface_Mg_ha**: total live surface fuel load (Mg/ha); includes live understory herbaceous vegetation, woody shrubs, and trees (height < 1.37 m)
- **herbs_Mg_ha**: fuel load of live herbaceous vegetation (Mg/ha); includes non-woody forb, graminoid, and non-vascular plant species
- **shrubs_Mg_ha**: fuel load of live woody shrubs (Mg/ha); includes woody shrub and subshrub species
- **conifer_seedlings_Mg_ha**: fuel load of live understory conifer trees (Mg/ha); includes conifer species (i.e., gymnosperms, Coniferophyta) with height < 1.37 m
- **broadleaf_seedlings_Mg_ha**: fuel load of live understory broadleaf trees (Mg/ha); includes broadleaf species (i.e., angiosperms, Magnoliophyta) with height < 1.37 m



### canopy_fuels.csv

This file contains stand-level post-fire canopy fuel profiles for each sampled plot. These data include all live and dead canopy trees (height ≥ 1.37 m). The following columns are included:

- **plot_id**: unique plot identifier in the format *site_plot#*
- **foliage_Mg_ha**: total foliage fuel load (Mg/ha); includes live and dead foliage on all individuals
- **foliage_Mg_ha_live**: live foliage fuel load (Mg/ha); includes live foliage on live individuals
- **foliage_Mg_ha_dead**: dead foliage fuel load (Mg/ha); includes dead foliage on live and dead individuals
- **branches_Mg_ha**: total branch fuel load (Mg/ha); includes all live and dead branches on all individuals
- **branches_Mg_ha_live**: live branch fuel load (Mg/ha); includes all live branches on live individuals
- **branches_Mg_ha_dead**: dead branch fuel load (Mg/ha); includes all dead branches on live and dead individuals
- **branch_1h_Mg_ha**: total 1-h branch fuel load (Mg/ha); includes all branches with diameter < 0.6 cm on all individuals
- **branch_1h_Mg_ha_live**: live 1-h branch fuel load (Mg/ha); includes live branches with diameter < 0.6 cm on live individuals
- **branch_1h_Mg_ha_dead**: dead 1-h branch fuel load (Mg/ha); includes dead branches with diameter < 0.6 cm on live and dead individuals
- **branch_10h_Mg_ha**: total 10-h branch fuel load (Mg/ha); includes all branches with diameter 0.6–2.5 cm on all individuals
- **branch_10h_Mg_ha_live**: live 10-h branch fuel load (Mg/ha); includes live branches with diameter 0.6–2.5 cm on live individuals
- **branch_10h_Mg_ha_dead**: dead 10-h branch fuel load (Mg/ha); includes dead branches with diameter 0.6–2.5 cm on live and dead individuals
- **branch_100h_Mg_ha**: total 100-h branch fuel load (Mg/ha); includes all branches with diameter 2.5–7.6 cm on all individuals
- **branch_100h_Mg_ha_live**: live 100-h branch fuel load (Mg/ha); includes live branches with diameter 2.5–7.6 cm on live individuals
- **branch_100h_Mg_ha_dead**: dead 100-h branch fuel load (Mg/ha); includes dead branches with diameter 2.5–7.6 cm on live and dead individuals
- **branch_1000h_live**: live 1000-h branch fuel load (Mg/ha); includes live branches with diameter ≥ 7.6 cm on live individuals
- **crown_Mg_ha**: total crown fuel load (Mg/ha); includes foliage and branches on all individuals
- **crown_Mg_ha_live**: live crown fuel load (Mg/ha); includes live foliage and branches on live individuals
- **crown_Mg_ha_dead**: dead crown fuel load (Mg/ha); includes dead foliage and branches on live and dead individuals
- **acfl_Mg_ha**: total available canopy fuel load (Mg/ha), defined as the sum of total foliage, dead 1-h branches, and half of live 1-h branches ([Reinhardt et al. 2006](https://doi.org/10.1139/x06-157)); includes all live and dead individuals
- **acfl_Mg_ha_live**: live available canopy fuel load (Mg/ha), defined as the sum of live foliage and half of live 1-h branches; includes live individuals
- **acfl_Mg_ha_dead**: dead available canopy fuel load (Mg/ha), defined as the sum of dead foliage and dead 1-h branches; includes live and dead individuals
- **cbd_kg_m3**: canopy bulk density (kg/m<sup>3</sup>), defined as the maximum 3-m running mean of the vertical canopy fuel profile ([Reinhardt et al. 2006](https://doi.org/10.1139/x06-157))
- **cbh_m**: canopy base height (m), defined as the lowest height at which canopy bulk density exceeded 0.04 kg/m<sup>3</sup> ([Cruz et al. 2004](https://doi.org/10.1093/forestscience/50.5.640), [Donato et al. 2013](https://doi.org/10.1890/12-0772.1), [Sando and Wick 1972](https://research.fs.usda.gov/treesearch/10605))
