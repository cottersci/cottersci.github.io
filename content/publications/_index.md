---
title: Publications
date: 2017-08-14T20:10:07-04:00
draft: false
Summary: ""
pinned: "false"
---

## Data-driven modeling reveals cell behaviors controlling self-organization during Myxococcus xanthus development

{{%
  figure src="/publications/PNAS2017/LS3909-LS3629-50-200msec-1secdelay.gif"
  caption="Example of cell trajectories extracted from a time-lapse movie. Each bright white dot is one cell, with a randomly colored trajectory path showing the cell's previous positions. For each high-fluorescent cell there are approximately 2,500 low-fluorescent cells surrounding it. Ellipses indicate aggregate positions detected using the weak florescence of the surrounding cells"
  width="75%"
  class="figure_centered"
%}}
#### Link to the paper: [PNAS 2017](http://www.pnas.org/content/114/23/E4592.short)

<!--more-->

Within the soil in your backyard lives a genus of bacteria known as *Myxococcus*, possibly one of nature’s earliest attempts at multi-cellular coordination. When starved, these bacteria coordinate their movement to generate a multicellular fruiting body used to help them survive the famine. By tracking the movement of fluorescent *Myxococcus* cells during fruiting body development, we were able to observe minute changes in cell movement and orientation relative to the location of the emerging fruiting body.

The GIF above shows a typical fluorescent cell tracking experiment we perform in the laboratory. The entire surface within view is covered with a layer of bacteria 3-5 layers thick, known as a biofilm. To track the movement of individual cells within the biofilm, we added 1 fluorescent cell for every 2,500 cells in the biofilm. When imaged using a UV light source, the fluorescent cells light up brightly, while the rest stay dark, allowing the movements of individual cells within the biofilm to be seen. The resulting time-lapse images are then analyzed using custom computer vision algorithms to quantify the movement patterns of each individual fluorescent cell.

To track the forming fruiting bodies, the other 2,500 cells are modified so that they are slightly fluorescent. You can see these cells as the smoother changes in background brightness in the GIF. Brighter areas indicate higher cell densities. Image filtering is used to extract the highly fluorescent cells for tracking while also extracting the background fluorescence to estimate cell density within the biofilm. From the cell density estimation, the aggregates can be detected and tracked. The boundaries of aggregates are approximated with ellipsis in the above GIF. Using the combined information about individual cell movement and the environment in which the cells were moving, we were able to identify behavior/cue correlations important for coordinating cell movement to generate aggregates.

The movements of individual cells within the population appeared almost random. Uncovering the coordinating mechanisms required identification of small changes in cell behavior relative to their location in the environment that, when averaged over thousands of cells, allows for self-organization. Computer simulations driven by the cell tracking data were then used to test if each of the identified cell behavior/cue combinations was important for aggregation.

In the end, the computer simulations revealed that three behaviors were necessary and sufficient for the pattern to form. Early on, side-by-side alignment of many cells created prepatterns, some of which coordinated movement and provided enough topological detail to define the locations of the fruiting bodies. Then, motility of cells at the aggregation foci became sluggish leading to a buildup of cells in those locations. Outside the growing aggregates, cells biased their movement toward the aggregation foci.

The work is important in that none of the cues altering cell behavior are known, nor are the mechanisms by which the cells respond to these cues. Nevertheless, the simulations make strong predictions about the emergent pattern-building process that can be followed up by examination of mutants that lack one of these four behaviors. The results also suggest a more general role for these three behaviors in other patterning processes such as wound healing and tumor metastasis.

#### Other Press
* [npj's Biofilms and Microbiomes blog](http://npjbiofilmscommunity.nature.com/users/7272-ben-libberton/posts/17212-still-learning-from-myxococcus)

#### Acknowledgements
*This article is based off an unpublished press release Dr. Lawrence Shimkets and I wrote. I thank Dr. Shimkets for his time and effort in editing and refining the original text*
