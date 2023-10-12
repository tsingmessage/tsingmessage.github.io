---
layout: page
title: AI-based association analysis
description: We developed a novel AI tool to overcome the interpretability and confounding issues in deep-learning-based association analysis.
img: assets/img/0031.jpg
importance: 3
category: methodology
related_publications: 24th international conference on Medical Image Computing and Computer Assisted Intervention
---

AI has greatly enhanced medical image analysis, yet its use in epidemiological imaging studies remains limited due to visualization challenges in non-linear models and confounder control. Addressing this, we introduce an AI method emphasizing semantic feature interpretation and resilience against multiple confounders. Our approach's merits are tested in three scenarios: 1) extracting confounder-free features from a 2D synthetic dataset; 2) assessing the link between prenatal alcohol exposure and children's facial shapes using 3D mesh data; 3) exploring the relationship between global cognition and brain images with a 3D MRI dataset.
The scripts for this project can be found in <a href="https://gitlab.com/radiology/compopbio/ai_based_association_analysis">this Gitlab link</a>.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0032.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The distribution of the 2-D latent space for the synthetic images in the test set of Experiment 1, and the eleven reconstructed images sampling along the brightness-related vector, (a) without (i.e., vector 𝑝⃗) and (b) with correction (vector 𝑝∗⃗) for the confounding of circle radius, together with the predicted brightness 𝑡̂ (Eq. 6 and Eq. 7). Z1-axis: the first dimension of the latent space; Z2-axis: the second dimension. Each data point in the latent space represents an input image, which is denoted by its radius and brightness. After training, eleven frames were reconstructed by sampling eleven points along the vector 𝑝⃗ and 𝑝∗⃗ (Eq. 6, Eq. 7) to visualize the confounding effects.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0033.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Association between global cognition and brain images with a 3D MRI dataset. Reconstructed supratentorial modulated grey matter maps using the sampled latent features along the direction of increasing g-factor (a) without correcting for confounders, and (b) with correcting for age, sex, and educational years. The results are generated using the semi-supervised model, averaged over the five folds, and masked out the statistically non-significant region. Color bar shows the direction and magnitude of the changes of GM density.
</div>
