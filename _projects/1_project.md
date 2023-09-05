---
layout: page
title: Automated three-dimensional analysis of facial asymmetry
description: We developed an automated pipeline for quantifying facial asymmetry from three-dimensional craniofacial images.
img: assets/img/0011.jpg
importance: 1
category: methodology
related_publications: einstein1956investigations, einstein1950meaning
---

We developed an automated pipeline for quantifying facial asymmetry from three-dimensional craniofacial images. The process begins by taking the facial shape of each subject as input, after which a mirrored reflection is generated. This mirrored image was then automatically aligned with the input via rigid registration. The vertex-wise distance between these two aligned facial shapes was then computed. Finally, two quantitative outcomes were produced for each subject: 1) a facial heatmap based on the distance where zero-error regions are perfectly symmetric while higher-error regions are more asymmetric; 2) a mean facial asymmetry (MFA) based on the mean of the error. This pipeline has been implemented as an inline function within [CraniumPy](https://github.com/T-AbdelAlim/CraniumPy).



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0012.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The developed automatic pipeline for 3D facial asymmetry measurement. Red color in the outcome facial heatmap means expanding outward with respect to the contralateral half.
</div>
