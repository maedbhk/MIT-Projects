---
title: Pre-OHBM Gradients Workshop
---

## Session 1: Methods
### Superficial white matter
* Underneath grey matter, has been described in anatomical studies
* SWM in development and aging and disease, temporal lobe epilepsy, AD, and ASD
* Current methods to study SWM: surface based tractography, mask based methods (Registration-dependent), laplacian
	* disadvantages, computationally expensive, difficult to implmeent, multiple dependencies
	* new method to identify SWM
	* 7T MRI dataset - high res data, 3 sessions etc. 
	* solves laplacian field, generates surfaces below grey matter (can be many surfaces)
* microstructural intensity profiles derived from each SWM surface

### Biologically annotated brain connectomes 
* connectomes: network of nodes and edges
* annotated connectomes: thus far, pairwise relationships between regions
* homophily in annotated connectomes: nodes that have degree in a connectome tend to be more connected
	* homophily can be quantified using the assortativity coefficient: the correlation between annotation values of connected nodes
* spatial constraints of the brain: annotations are spatially autocorrelated and connections have a wiring cost (most connections are short range)
* what is the relationship between local biological annotations and brain connectivity? 
	* paths: what bio attributes do signals encounter along communication paths? 
	* can biological annotations enhance models of the brain? 
* annotation-enhanced models of the brain: 
	* biophysical models
	* heterogenous models
* models of brain diseases
* neuromaps toolbox: hosts brainmaps from lots of people etc. 

### Principles of white matter organization in relation to cognition in youth
* Speaker from Ted Satterthwaite's group
* surface gradients: lower order sensory processing - complex cognitive functions
* braod categories of gradients: function - structural: microstructure (myelination) - development:fluctuation amplitude (age effect)
* regional variation in white matter
	* volumetric studies
	* tractography
* during youth, cortical white matter is extensively remodeled and expands a lot
* evidence from DTI suggests asyncrhonous maturational timing 
* limitation: anatomically pre-defined atlases
	* discrete anatomical bundles = discrete anatomical regions
* what's missing: bundle-based approaches do not caputure spatial covariance that may exist across distribute white matter locations
* certain areas may share similar strutural profiles even though they belong to diff. anatomical bundles
* structure of subregiosn wtihin the same bundle may vary significantly. 
* spatial organization is likely driven by syndrhonized matural processes
* dataset: philadelphia neurodevelopmental cohort (PNC)
	* white matter structure has many crossing fibers that aren't well represented in conventional methods. use fixel-based analysis, more accurate than conventional DTI
	* fixels (FBA) - higher resolution, increase feature space - allows for more accurate white matter structure
* how do you capture covariance across white matter structure?
* non-negative matrix factorizatoin (NMF): similar to PCA, but doesn't maximize variation in first few components, but get a parts-based representation. 
* delineate associations with age and cognition
	* use generalized additive models
* results:
	* delineate the spatial and temporal organization
	* 14 components: capture white matter structure
* white matter structure components show widespread development: corpus callosum, arcuate, and splenium
* developmental gradient: early maturation, inferior and posterior
* superior cerebellum, vermis, cingulum, early maturation of white matter
* intermediate regions: pareitnal, splenium (12-16 years maturation)
* late maturation: end of adolescence (anterior and superior matures later)
* there might be a hierarchical pattern of age-related changes in white matter structure

## Session 2: Beyond the Neocortex
* Striatal gradients in health and disease
* non-invasive method for investigating the dopaminergic system (in striatum)
* biomarker for altered dopaminergic signaling at the single-subject level
* psychosis: PET studies indicate increased striatal dopaminergic signaling in psychosis. 
* rs-fMRI studies have linked altered cortico-striatal connectivity to both psychosis and subclinical psychosis-like experiences
* analysis of both 2nd cortico-striatal and 3rd dopaminergic connectivity gradient
* psychosis 2nd connectivity gradient
* next steps: investigate striatal gradients in other dopamine-associated conditions such as ASD and ADHD. 
	* push connectompic mapping in the temporal domain
* looking at other regions, find the same pattern - makes sense that you would find this

CMI Autism Spectrum Center Director: Adriana Di Martino - https://childmind.org/science/fundamental-neuroscience/autism-center/
Breanne Kearney bkearne3@uwo.ca - send paper on fear conditioning in the cerebellum

## Session3 3: Flash Talks
* identifying spatiotemporal changes in cortical neurodevelopment in postmortem and in vivo data
* multi-modal, area- and depth-wise characterization of cortical structure throughout development
* baby connectome project
* generation of a normative model of intracortical development
* microstructure increases across cortical depths, but increases are selectively more pronounced in deeper layers

hierarchical neurodevelopment
* emergence of sensory-association axis

## Session 4: AI 
* Sofie valk group

* excitation and inhibition
* brain changes in adolescence: changes in excitatory and inhibitory balance - implication for neurodevelopmental disorders
* lots of E/I balance comes from animal models
* challenges of studying excitatoin and inhibition in humans
* simulations that map on to imaging data
* using biophysical network modeling of rs-fMRI, how does excitation-inhibition develop? 
* datasets: PNC (n=764) and IMAGEN (n=149, longitudinal)
* model-simulation optimization: how do we go from imaging data to E/I balance in each area? 
* development: sensorimotor areas develop early and association matures later

## Sensorimotor-association axis and sex differences
* Sofie valk group
* developmental and evolutionary expansion
* inter-individual variability of S-A axis is lacking
	* focus on sex differences
	* intra-individual differences
* although brain size shows robust sex differences, it is unclear whether it differentially shapes functioanl cortical organization between sexes through altered cortical mophometry
* brain size is a major scaling factor across evolution and development
* sex differences present at the poles of the S-A axis. females > DMN and males > sensorimotor network
* differences in cortical mophometry - responsible for differences in cortical organization? 
* cortical mophometry supports function
	* primary regions - short range connections
	* association - long range connections 
* sex differences in S-A axis? 
	* morphometric correlates of S-A axis
	* test first for effect of brain size on S-A axis (ICV, TBC, Total SA) - total SA most widespread effect on S-A axis
	* sex differences in 23% of regions - DMN, frontoparietal
* sex differences in S-A reflect differences in morphometric correlates? 
	* sex differences in cortical morphometry explain little of the variance in S-A axis
* S-A axis of multimodal organizational hierachy 
* sex differences in 1.2% of all functional connectiviyt measures (schaefer x schaefer networks)
* females show a more integrated DMN compared to males
* sex dfiferences in S-A axis do not apear to be systematically explained by diffferneces in brain size, microstructural organization or mean geodesic distance
* intra-individual differences:
	* Dense sampling - MyConnectome study and Midnight scan club
* mechanisms underpinning functional variability? 
	* the brain interacts with the endocrine system
	* pritschet et al. (2020) and Grotzinger et al. (2023) - jacobs lab data
	* intra-/inter-individual differences in variability
	* inter-individaul differences in variability - higher variability in male subject (case study)
	* local-level effects on S-A axis loadings
* don't overinterpret results - there are more similarities than differences. the brain is not sexually dimorphic. 

## Using a neural state-space to understand cognition and behavior
* Samyogita Hardikar
* Gradients allow us to summarize variability in a compact manner
* Margulies et al. (2016) PNAS - first gradient paper. Axes of functional variation in the brain. Motor-to-association
* Third gradient separates systems DMN from multiple-demand networks
* Axes of functional variation in the brain
* brain-wide associations of personality traits only possible with lots of data
* do mass-univariate approaches give a "brain-wide" picture
	* no, just smootheed group regions
* can rest/any one task condition provide all the information? 
* personality dimensions can be conceptualized as "if-then" rules
	* not all traits will be expressed in every given situation
	* intrinsic connectivity (functional organization) + context
* HCP Young-Adult s1200
	* task fMRI: WM, Gambling, Motor, Language, social cognition, relational processing, emotion
	* trait measures (neo-ffi) - big 5 traits: neuroticism, openness, conscientiousness, extraversion, agreeableness (minimally preprocessed 2mm smoothing CIFTI)
	* neural state-space: primary-associatoin; motor-visual; DMN-FPN

## Procrustes alignment
* solve the issue of gradient alignment