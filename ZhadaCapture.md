---
layout: page
title: Was the Zhada Basin captured by the Sutlej River?
permalink: /Research/ZhadaCapture
---

# <u>Was the Zhada Basin captured by the Sutlej River?</u>

| ![Overview Map of Large Capture Events.](./Images/HimalayaCaptureAnalogs_240116b.png) | 
|:--:| 
| *Regional maps of the northwest and central Himalayas. (A) Map of captured basins (blue polygons) and the Sutlej study area (yellow dot). (B) Map of the major geologic units and fault systems. MFT - Main Frontal Thrust, MBT - Main Boundary Thrust, MCT - Main Centrarl Thrust, STDS - South Tibetan Detachment System, GCT - Great Counter Thrust.* |

The Himalayas are one of the most studied mountain ranges on Earth, however our understanding of how these mountains, and the river systems that drain them, have changed over time remains incomplete. For example, several studies have identified river networks that have experienced drainage capture (<i>blue polygons in A above</i>), which occurs when the drainage divide separating two networks is breached, altering flowpaths such that one network is "captured" by the other. The exact mechanism, or mechanisms, that caused these captures in the Himalayas remains elusive, preventing us from fully understanding the significance of these events with respect to the evolution of the mountain range.   

 In my work, I focused on a proposed capture event within the Sutlej River network. Today, the Sutlej River is one of the largest rivers that crosses the Himalayas. The river originates in southern China before flowing through the Zhada Basin, which is a high-elevation sedimentary basin believed to have once contained a vast lake. One hypothesis for this transition from a lake to a through-flowing river in the Zhada Basin is that the Sutlej River captured the basin within the past million years. This hypothesis had not been rigorously tested, but if it were the case, then it is likely that the Sutlej River incised across the Himalayan range crest, breaching the existing topographic barrier that helped form the lake.

| ![Map of knickpoints, generated in QGIS.](./Images/Figure_3.png) | 
|:--:| 
| *(A) Map of identified knickpoints in the Zhada basin. Knickpoints between 4350-4550m above sea level are radially dispersed and lie in close proximity to the 4500m contour. (B) Distribution of knickpoint elevations. A prominent peak between 4350-4550m suggests these knickpoints are transient and may have been initiated by drainge capture. Smaller peaks between 3800-4100m and 5000-5500m are thought to result from contrasts in rock type and the extent of alpine glaciers, respectively. (C) Zoomed in example of transient knickpoints separating zones of higher erosion rates (streams with high steepness) and lower erosion rates (presence of geomorphic surface and streams with low steepness).* |

By using at a digital elevation model (DEM) of the Zhada Basin, we can begin to address this hypothesis. Below is a figure showing the spatial distribution of identified knickpoints, or slope breaks, along a river channel within the Zhada Basin (<i>A</i>). Most knickpoints are found within one of three elevation ranges, with an abundance of knickpoints between 4350-4550m above sea level (<i>orange region in B</i>). Two predicted outcomes of drainage capture are: (1) knickpoints, representing the front of a propagating wave of increased river erosion, are generated upstream from where capture occurred and (2) these knickpoints are located at similar elevations. At first glance, it appears the knickpoints between 4350-4550m satisfy these two predictions, however we also need to check whether the knickpoint X,Y locations match what would be expected if they were capture-generated.

| ![Knickpoint model results, generated using QGIS and Matlab.](./Images/ModelExample_230420a.png) | 
|:--:| 
| *Example of knickpoint modeling results. (A) Cartoon example of geomorphic differences in stream channels downstream and upstream of transient knickpoints. Stream segments downstream from knickpoints between 4350-4550m above sea level are steeper than segments upstream from the knickpoints. (B) Map of the Zhada Basin with observed knickpoints between 4350-4550m above sea level and modeled knickpoint locations. Note the close proximity of the two datasets. (C) Observed v. Modeled upstream distances of knickpoints between 4350-4550m above sea level.* |

To test this hypothesis, I wrote several Matlab scripts [(GitHub Link)](https://github.com/BPenserini/KPPropagation) to automate simulations of the expected dynamics of capture-generated knickpoints within the Zhada Basin. In the figure above, modeled knickpoint locations match very well with the observed knickpoint locations, with modeled knickpoint propagation distances within 2%, on average, of observed propagation distances). This finding suggests that the spatial distribution of observed knickpoints at elevations between 4350-4550m matches what we would expect if these knickpoints were generated by drainage capture, which leads us to infer that the Sutlej River did, in fact, capture the Zhada Basin.

If you would like to learn more about this project, including how we were able to better constrain the timing of this event and the associated eroded volumes, please check out the [full manuscript](https://onlinelibrary.wiley.com/doi/10.1002/esp.5705) published in <i>Earth Surface Processes and Landforms</i>.

<i>Penserini, B.D., Morell, K.D., Codilean, A.T., Fülöp, R., Wilcken, K.M., Yanites, B.J., Kumar, A., Fan, S., Mearce, T., 2023. Magnitude and timing of transient incision resulting from large‐scale drainage capture, Sutlej River, Northwest Himalaya. Earth Surf Processes Landf esp.5705. https://doi.org/10.1002/esp.5705</i>
