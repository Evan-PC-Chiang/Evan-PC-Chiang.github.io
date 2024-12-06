---
layout: post
title: Insight of the Land Subsidence in the Western Taiwan Coastal Area by Using PSInSAR Technique
date: 2020-11-17 10:14:00-0400
description: Geoscience 2020 @Taipei New Horizon, poster No. P17-0052
categories: Conference Result
last_updated: 2023-08-23 20:45:15-0400
giscus_comments: true
related_posts: false
toc:
  sidebar: left
---
<p style="text-indent: 0em;"><span style="font-size:14px;"><a href="https://evan-pc-chiang.github.io/">Ping-Chen Chiang</a><sup>1*</sup>, <a href="https://raychuang0.wixsite.com/ntugeog">Ray Y. Chuang</a><sup>1</sup>, <a href="https://researchoutput.ncku.edu.tw/en/persons/chih-heng-lu">Chih-Heng Lu</a><sup>1**</sup></span><br />
<span style="font-size:9px;">1: Department of Geography, National Taiwan University, Taipei, Taiwan.<br />
*: Currently at Department of Earth &amp; Atmospheric Science, Indiana University Bloomington, Indiana, USA.<br />
**: Currently at Department of Earth Sciences, National Cheng Kung University, Tainan, Taiwan.</span></p>



## Introduction

Land subsidence is a severe problem in western Taiwan. The modern geodetic data indicates the velocity of this area can be up to 6.5cm/yr. Leveling and GPS can offer us accurate point data, but the lack of planar data makes it hard to comprehend the land subsidence distribution. Thus, we can get the land subsidence distribution by using PSInSAR.
## Baseline
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/brep_before.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Baseline before 2016 southern Taiwan earthquake
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/brep_after.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Baseline after 2016 southern Taiwan earthquake
</div>


## Procedure

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/procedure.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Data processing procedure
</div>


Since several factors might distort PSInSAR, we use GPS to constrain the velocity of the PSInSAR LOS result. After GPS fitting and removing the antenna signal from the GPS time series, we can constrain the PSInSAR data by converting GPS data into LOS direction. By doing this, the LOS velocity of ascending (VA) and descending (VD) can reveal truth ground displacement (LOS direction). The vertical (Vv) and east-west (VE) velocities can be solved by the following formula (Tofani et al., 2013):

$$
\begin{bmatrix}
cos\theta _{A} & sin\theta _{A} \\
cos\theta _{D} & sin\theta _{D}
\end{bmatrix} \begin{bmatrix}
V _{V}\\
V _{E}
\end{bmatrix} = \begin{bmatrix}
V _{A}\\
V _{D}
\end{bmatrix}
$$

## Velocity Field

We should avoid earthquake events because of the coherence problem if we want a better PSInSAR result. In this case, we separate all sentinel-1A/B images into two periods—before and after the 2016 Meinong earthquake—to achieve this.

### Line of Sight Direction

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/LOS.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


From left to right are (A) ascending pre-earthquake, (B) ascending post-earthquake, (C) descending pre-earthquake, and (D) descending post-earthquake, respectively. Yunlin and Pingtung have more than 30mm/yr LOS subsidence. Also, the velocity changes in Tainan and Kaohsiung after the Meinong earthquake are very significant.

### Horizontal and Vertical Direction

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/VH.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


From left to right are (A) pre-earthquake east-west, (B) post-earthquake east-west, (C) pre-earthquake vertical, and (D) post-earthquake vertical, respectively. There are velocity differences between the two periods, especially in vertical velocity in southern Taiwan. We can see high matches between PSInSAR vertical velocity and fault data (Fault data from J. Bruce H. Shyu). Meanwhile, the subsidence region seems to become more significant and profound in Yunlin and Pingtung.

P.S. Misfits are due to the lack of an N-S direction component in PSInSAR data.

## Timeseries Comparison

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/TS.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


Since this study focus on the plain area, GPS and PSInSAR seem well fitted. The figure shows some of the GPS stations within the whole PSInSAR area. PSInSAR variation gets more extensive in the mountain area, so blackout those results in the mountain area.

## Conclusion

SAR—different from GPS—can give us planar data and shows surface displacement instead of point displacement. This information reveals surface displacement, including land subsidence and uplift; data density can indicate fault location and help us figure out new fault structures. Adding GPS data as a constraint can eliminate PSInSAR data distortion, making PSInSAR results more reliable for better understanding faults behaviors and surface deformation.

## Poster

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/post/PSInSAR/poster2020.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## Conference Info

<p style="text-indent: 0em;"><span><a href="https://cgs.gst.org.tw/Geosciences2020" target="_blank">Geoscience 2020 @Taipei New Horizon</a>, poster No. P17-0052</span></p>

