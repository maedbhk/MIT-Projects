---
title: Healthy Brains Network
---
## [Healthy brains](http://fcon_1000.projects.nitrc.org/indi/cmi_healthy_brain_network/)

### Overview
The Child Mind Institute has launched the Healthy Brain Network, an ongoing initiative focused on creating and sharing a biobank comprised of data from 10,000 New York City area children and adolescents (ages 5-21).

* Population: ages 5-21, children who likely have one or more psychiatric symptoms
* Data collected: 
    * MRI + fMRI: movies (~10 min), predictive eye estimation regression - 3444 participants
    * Phenotypic assessment - 4080 participants
    * Physical activity
    * Behavioral measures (questionnaires)
    * Family structures (stress, trauma)
    * Substance use/addiction
    * Cognition and language tasks
    * Disorder-specific questionnaires
    * Electroencephalography
    * Digital Voice and Video Recordings
    * Genetics
    * Actigraphy
    * Cognitive Tasks (e.g., sequence learning), naturalistic stimuli
    * Eyetracking: pupil dilation and eye position

![Phenotypic Assessment Protocol](http://fcon_1000.projects.nitrc.org/indi/cmi_healthy_brain_network/images/R9_assessments.png){fig-align="center"}

### Data Storage
* Which data are on openmind?
    * Imaging (rest, naturalistic)
    * Demographic info
    * Cognitive/Behavioral results
    * Clinical disorders
* What is the format?
    * raw, derivatives
* Which releases are available?
    * currently there are [10 releases](http://fcon_1000.projects.nitrc.org/indi/cmi_healthy_brain_network/sharing_neuro.html#Direct%20Down) of HBN imaging and phenotypic data
* Have imaging data been preprocessed?
    * fmriprep (no)
    * freesurfer (no)
    * first-level glms (no)
* MRI data have been preprocessed using Mindboggle and are available in S3 under the [directory](/fcp-indi/data/Projects/HBN/derivatives/Freesurfer_version6.0.0)
* Where are the data stored on openmind?
    * are these data being transitioned to datalad?
* How does a new user get access to the dataset?
    * anyone with gablab group permissions should be able to access the data

* directories on openmind - HBN
    * `/om4/group/gablab/data/hbn_bids`
    * `/nese/mit/group/sig/projects`

### MRI and fMRI Data Preprocessing
* Use [xcp-D package](https://xcp-d.readthedocs.io/en/latest/) to do post-processing of resting state data (basically picks up where fMRIPrep left off)
* This package also works on outputs from [minimially preprocessed HCP data](https://www.humanconnectome.org/study/hcp-lifespan-development/data-releases)