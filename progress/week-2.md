---
title: Week 2
---

I liked the idea Satra presented in lab meeting (last week I think) about documenting steps of a project, from conception to publication. In my position now, I thought it would be a good opportunity to make this process transparent so I'm putting together a webpage (eventually hosted at [](https://maedbhk.github.io/MIT-projects)). I plan on integrating visualizations for projects as they're in progress and keeping a running log (in the form of weekly reports). Given that the overarching aim of future projects should address the question: "how is what we're doing applicable and useful for the broader community", I hope to be able to use this platform to create an interface that allows for clear communication of project aims, findings, and interpretations, to any interested parties.

## Project Guidelines (to have in mind throughout)
* Inform clinical outcomes through computational modeling
* Communicate importance and relevence of research findings to patient population whose biodata are being collected and analyzed
* Work with clinicians to offer risk assessment predictors to patients based on outputs of biologically-driven models
* Effectively communicate scientific uncertainty to both experts and non-experts alike
* Create models that are accessible to other researchers, FAIR, and demographically diverse
* Address ethical questions that may arise throughout the entire process: as studies are being designed, data analyzed, and results disseminated
* How can the results of this work be translated to a clinical application? 
* Are our findings clinically useful? If not, have we at least learned something interesting about the brain with this question?  

## Project Ideas
* 1) can unique cerebellar fingerprints dissociate neuropsychiatric and neurodevelopmental disorders, above and beyond what would be expected from cortical fingerprints? I think I'd be first interested in analyzing the structural data before addressing functional connectivity
* 2) inspired by RDoC, can we use topic models (e.g., latent dirichlet allocation) to identify latent clinical characteristics derived from HBN behavioral and/or cognitive measures (e.g., positive and negative affect scale, GRIT scale, Wechsler intelligence scale) with the goal of providing individualized risk assessments. 
* 3) If we can identify groups/clusters by modeling behavioral/cognitive characteristics, can we identify corresponding dissociable neural signatures (whole-brain, not necessarily cerebellum-focused)? 
* 4) Relative to the neocortex, are there differences across disorders in neural signatures/fingerprints from early childhood to adolescence? For example, in developmental disorders (e.g., adhd, autism) do we see more significant changes in cerebellum (as indexed by reduction in grey matter) during early childhood relative to corresponding changes in the neocortex.  

Next steps: 
- Once I get access to HBN, I want to do a summary analysis of the phenotypic assessment data to determine the scope of the data (e.g., do some power analyses)
- If it seems like there is a sufficient sample and enough complete behavioral measurements, I'll likely plan on testing cerebellar isolation and segmentation of a few pilot participants (not clear to me yet what technical challenges we may face using SUIT on a developmental dataset). 
- test some topic models on the HBN phenotypic assessment data
- I plan on publishing the website today at some stage so I'll slack you the link, hopefully that will be an easier way to get a sense of what I'm working on