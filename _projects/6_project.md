---
layout: page
title: Survival analysis
description: Predicting skin cancer risk from facial images with an explainable artificial intelligence (XAI) based approach. a proof-of-concept study
#img: assets/img/0061.jpg
importance: 6
category: application
related_publications: medRxiv2023
---
Check the online demonstration of this project [here](https://huggingface.co/spaces/CoPoBio/skin_cancer_risk_prediction).

Efficient identification of individuals at high risk of skin cancer is crucial for implementing personalized screening. We present a neural network-based explainable artificial intelligence (XAI) approach for skin cancer risk prediction based on facial endophenotypes obtained from 2D facial images, and compare its efficacy to 18 established skin cancer risk factors using data from the Rotterdam Study. Among the 2,810 participants (mean Age=68.5 ± 9.3 years, average Follow-up=5.0 years), 228 participants were diagnosed with skin cancer at various body locations after photo acquisition. In the skin cancer survival analysis, our XAI approach achieved superior predictive accuracy based on facial endophenotypes (c-index=0.72, SD=0.05) for skin cancer diagnosis on any body location, outperforming that of the known risk factors (c-index=0.59, SD=0.03). Furthermore, our XAI techniques indicated facial features such as a lower BMI and increased facial erythema are linked with higher risk of developing skin cancer. This proof-of-concept study underscores the high potential of harnessing facial images and a tailored AI approach as an advanced predictive alternative over known risk factors for identifying individuals at high risk of developing skin cancer.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0063.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Our XAI approach to generate synthetic facial images showing facial features related to a lower or higher risk of developing skin cancer.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0062.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Reconstruction of faces representing lower to higher risk for developing skin cancer on the face, and other body locations excluding the face, as well as anywhere on the body including the face. The synthetic faces shown in the figure were reconstructed via selectively decoding statistically significant facial endophenotypes in the survival analysis.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0063.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The risk prediction scores of subjects in the test set.
</div>
