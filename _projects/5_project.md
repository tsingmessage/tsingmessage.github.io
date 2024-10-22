---
layout: page
title: Genetic studies
description: A fully data-driven approach for genome-wide-association stuides (GWAS) with image-based phenotypes
#img: assets/img/0051.jpg
importance: 5
category: application
related_publications: einstein1956investigations, einstein1950meaning
---

This study introduces a pioneering pipeline that combines AI-driven image phenotyping with combine-GWAS ([C-GWAS](https://www.nature.com/articles/s41467-022-35328-9)) techniques to enhance the genome-wide association studies (GWAS) of image-based complex traits. Conventional GWAS struggles with image-based phenotypes due to its reliance on 1-dimensional traits and huge number of redundant phenotypes defined. To overcome this limitation, we leverage AI-generated endophenotypes as proxies for complex image traits. Unlike previous data-driven endophenotype approaches, our method integrates C-GWAS to establish a robust connection between (the combined) endophenotypes and genetic variants. Applied to facial shape data from the combined of two cohorts (N=7,309), our approach uncovers total 43 genomic loci and with their visual correlates via facial heatmaps and 12 of them are novel. Significantly, C-GWAS outperforms single-trait GWAS in AI endophenotypes. Furthermore, we address privacy concerns in multi-cohort studies by implementing federated learning techniques, eliminating the needs for data sharing. This innovative pipeline offers a comprehensive solution for studying image-based complex traits within the GWAS framework.


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
