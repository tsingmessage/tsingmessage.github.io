---
layout: page
title: Genetic studies
description: A fully data-driven approach for genome-wide-association stuides (GWAS) with image-based phenotypes
#img: assets/img/0051.jpg
importance: 5
category: application
related_publications: einstein1956investigations, einstein1950meaning
---

Genome-wide association study (GWAS) has been pivotal in identifying genetic loci associated with specific phenotypes of scientific interest. Although highly effective in various applications, the conventional GWAS framework is inherently designed for single phenotypic traits, posing significant challenges when applied to complex medical image-based phenotypes. Defining phenotypes that capture the full variance of an image is difficult, requiring careful consideration of multiple testing corrections due to the large number of correlated phenotypes, and making the interpretation of results intractable.

Throughout the literature, several strategies have been proposed to tackle these challenges. One approach involves the direct utilization of each pixel or voxel within an image as a phenotype for GWAS, while another entails deriving prior-defined measurements from images as phenotypes. For example, the derivation of facial landmarks from facial images, and the region-of-interest volume from brain MRI scans. Although these strategies yield commendable outcomes with a large sample size, the real potential lies in seeking solutions that delve into image phenotypes in a more data driven manner, which goes beyond a priory defined knowledge.

Recent breakthroughs in artificial intelligence (AI) models have demonstrated great data-driven capabilities in preserving essential information while reducing high-dimensional image data into low-dimensional representations. This pivotal advancement has inspired pioneering researchers to leverage AI-derived low-dimensional representations, namely endophenotypes, as phenotypes for GWAS. Notably, this approach has proven fruitful in various contexts, such as unsupervised autoencoder-based endophenotypes for 3D brain images and 3D cardiac mesh images, self-supervised contrastive learning for molecular imaging, and transfer learning for retinal fundus images. However, so far only single-trait GWAS has been applied to endophenotypes, the potential of combing multiple endophenotypes has not yet been explored. Given that a SNP might have pleiotropic effects on multiple endophenotypes, we propose to combine the effects of multiple endophenotypes by using the combine-GWAS [(C-GWAS)](https://www.nature.com/articles/s41467-022-35328-9) approach. This approach is known for its capacity to augment the relationship between phenotypes and genetic variants by fusing multiple phenotypes. 

Another important concern in the AI-based phenotyping approaches  is the need of sharing individual data when conducting collaborations with multiple cohorts. Such collaboration is especially essential for conducting any well powered GWAS analysis. The underlying reason for this issue lies in the nature of the AI based data-driven approaches, where (endo)phenotypes are determined by the distribution of the local training data. If not sharing individual data in the training of model parameters, the definition of phenotypes differs from one cohort to another, and thus it will be difficult to analyse multiple cohorts. To address this, we propose to address scenarios involving multiple cohorts by harnessing federated learning techniques, eliminating the requirement for sharing image data, but obtaining integrated model parameters  

In summary, we propose a pipeline (Figure 1) to unlock the potential of image-based complex traits within GWAS through a synergistic fusion of data-driven AI phenotyping techniques and advanced statistical methodologies (i.e., the C-GWAS). To empirically exemplify its practical suitability, we applied the proposed AI pipeline to facial shape data from the Generation R Study (N=3,314) and the Rotterdam Study (N=3,995). We exploited the federated learning techniques to derive consistently defined 200 facial endophenotypes from two cohorts. Further GWAS, meta-analysis and C-GWAS not only uncovers novel genomic loci within a mediocre study population but also visually interprets associated phenotypes through facial heatmaps.  Furthermore, by integrating techniques from federated learning, we also demonstrate the success in our pipeline to collaborate more data from multiple cohorts to reach a better power with a large sample size.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0051.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The framework of our pipeline, including AI-based phenotyping, single-trait GWAS, and C-GWAS.
</div>



Figure below shows the Manhattan plot of our c-GWAS results, together with facial phenotypes associated with each leading SNP. In total of 43 genomic loci were identified, of which 12 have not been previously reported in existing studies.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/0052.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Manhattan plot of our c-GWAS results. Red areas refer to inward changes while blue areas refer to outward changes of the face with respect to the geometric center of the head.
</div>
