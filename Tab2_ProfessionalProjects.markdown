---
layout: page
title: Professional Projects
permalink: /ProfessionalProjects/
---

# <u>Landslide Volume and Mobility Analysis (U.S. Geological Survey)</u>

As a Pathways Intern for the U.S. Geological Survey, I assembled and analyzed a dataset of landslide characteristics to help improve assessments of long-term risk for wildfire burn areas. I developed a new workflow using density-based clustering (DBSCAN) in ArcGIS Pro to identify landslide source areas, which facilitated exploratory analyses of the relationships between landslide volume and mobility. I conducted exploratory analyses using statistical Python packages (NumPy, pandas, matplotlib, seaborn, scikit-learn, statsmodels, and SciPy) and assembled them in several Jupyter Notebooks to produce clear, well-documented, and resusable templates. All figures shown below were generated using Python.

<p align="center">
  <img width="" height="" src="./Images/LandslideOutletSlopeAreaExample.png">
</p>

The above plot shows the relationship between the topographic gradient, or slope, and the upstream drainage area where mapped landslides terminate (what I will call the "Landslide Outlet"). Since slope-area data is usually noisy, it is common practice to analyze binned average values, which are shown in brown. Grey points correspond to all Landslide Outlets within our dataset. We can see that most landslides terminate at drainage areas less than ~100,000 m<sup>2</sup>.

In the following plot, I've added the binned slope-area values for landslide source areas (green) and portions of the landcape that are occupied by channels that are formed by debris flow erosion or river incision (blue). It's common to define the transition from channels dominated by debris flow erosion to fluvial channels as the upper boundary of the "roll-over" in the binned slope-area curve, which is about 25,000 m<sup>2</sup> in our dataset. What we notice is that landslide source areas occur at about the same topographic slope, no matter where it is in the landscape (i.e., across a wide range of drainage areas), and the binned slope-area values for landslide outlets only overlap with the binned slope-area values for channels at drainage areas >1 km<sup>2</sup>.
 
<p align="center">
  <img width="" height="" src="./Images/LandslideFluvialSlopeAreaExample.png">
</p>

This seems to suggest that very few landslides actually flow into fluvial channels, where the landslide material can be more easily transported by surface runoff, and most landslides just redistribute their material within the hillslopes, which we define as portions of the landscape where drainage area is \<25,000 m<sup>2</sup>. We can see this more clearly in the following bar chart, which shows the number of landslides that deposited in fluvial channels and the number of landslides that remained on hillslopes.

<p align="center">
  <img width="" height="" src="./Images/LandslideOccurrenceGroupByRegime.png">
</p>

This, however, does not tell the full story. If we look at the volumes of material corresponding to the landslides in the chart below, we see that much more material is being redistributed by landslides with outlets in fluvial channels. This implies that there are many small landslides in our dataset that redistribute material within hillslopes, never making it to fluvial channels. Larger but less frequent landslides comprise the bulk of the total volume mobilized in landslides, with this material being deposited in channels where surface runoff can more easily transport it downstream.

<p align="center">
  <img width="" height="" src="./Images/LandslideVolumeGroupByRegime.png">
</p>

On the left side of figure below, I show three kernel density plots corresponding to volume distributions by source area elevation within the Romero Creek watershed. These distributions correspond to: (1) all landslides, (2) landslides with outlets on hillslopes (\<25,000 m<sup>2</sup>), and (3) landslides with outlets in fluvial channels (>25,000 m<sup>2</sup>). On the right is an elevation profile of the Romero Creek mainstem, along with the underlying geology. In this figure, we can start to see how the landslides redistributed material within the watershed. For example the Juncal Formation, which is found at higher elevations, sourced a large amount of landslide material that ended up in fluvial channels. This suggests that the Juncal may generate larger, more mobile landslides. Additionally, landslides that occur at lower elevations are slightly more likely to remain on hillslopes, even though they predominantly terminate in fluvial channels. This may imply that landslides at lower elevations within the Matilija and Cozy Dell Formations have a greater impact on increasing the hazard of future landslides, since they have a greater propensity to accumulate material in areas that can fail in future events.

<p align="center">
  <img width="" height="" src="./Images/RomeroCreekLandslideVolumeSchematic.png">
</p>

<i>This work is still in progress, with a manuscript currently in preparation.</i>

<i>Thomas, M.A., Lindsay, D.N., Rossi, R.K., Kostelnik, J., Rengers, F.K., Kean, J.W., Schwartz, J.Y., Swanson, B., Oakley, N.S., Richardson, P., Graber, A.S., Morelan, A.E., Ritchie, A.C., Warrick, J.A., Rotche, L., Penserini, B.D., Slaughter, S.L., 2023. Exploring controls on landslide occurrence across a patchwork of burned areas in southern California (USA). Presented at the 2023 AGU Fall Meeting, San Francisco, CA.</i>

<i>Penserini, Brian D., Francis K. Rengers, Matthew A. Thomas, et al. “Reloading the Channel Network through Postfire Shallow Landsliding” (in prep). </i>



