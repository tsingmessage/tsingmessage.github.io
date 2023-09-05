---
layout: page
title: Geometric deep learning on 3D mesh for derivation of endophenotypes
description: AI endophenotypes were derived, and conventional statistical analysis can be applied to these endophenotypes, in scenarios of epidemiological or genetic studies.
img: assets/img/0021.jpg
importance: 2
category: methodology
related_publications: einstein1956investigations, einstein1950meaning
---

After the registration of the facial images, each facial mesh has the same vertex number and edge connectivity. Thus, a 3D graph convolutional autoencoder can be applied to these facial meshes for dimensionality reduction. The low-dimensional representations are defined as endophenotypes. By decoding (one, or multiple) these endophenotype(s) via the docoder, the visual representation of endophenotype(s) can be shown with a faical heatmap, where red areas refer to inward changes while blue areas refer to outward changes of the face with respect to the geometric center of the head. Conventional statistical analysis can be applied to these endophenotypes, in scenarios of epidemiological or genetic studies.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0022.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Interpreting the representation of one endophenotype via decoding. Right: Visual interpretation of endophenotypes sorted from major to minor effects on the face.
</div>
