---
title: ABCD
---

## [ABCD](https://nda.nih.gov/abcd/)

### Overview 
The ABCD Study is a prospective longitudinal study starting at the ages of 9-10 and following participants for 10 years. The study includes a diverse sample of nearly 12,000 youth enrolled at 21 research sites across the country.

* Population: (n=12,000) Longitudinal study (starts at ages 9/10 for 10 years)
* Brain development: structural, task fMRI, resting state fMRI)
* Social, emotional, cognitive development, substance use and attitudes, physical health, environmental factors
* Local databases have been linked with ABCD dataset providing info about environment, poverty, pollution, school, policy for example [useful in providing context]

### Downloading Data
* See this community collection [(ABCC)](https://collection3165.readthedocs.io/en/stable/) on derivatives from ABCD 
* To download data, see this tutorial from [ABCD-ReproNim](https://github.com/ABCD-ReproNim/exercises/blob/main/project_month_prep/downloadABCD.md)
    * If the Jupyterhub (that contains NDA-tools) isn't working, just create a conda environment, which includes the relevent library (e.g., NDA-tools)
        * > example environment.yml
        ```
        name: abcd
        channels:
            - conda-forge
            - defaults
        dependencies:
            - pip
            - pip:
            - nda-tools
        ```
        * To create conda environment run: $ conda env create -f environment. yml 
        * To download data run: $ downloadcmd -dp <package_id> -d ABCD4
* [Download DCAN Labs ABCD-BIDS data](https://github.com/DCAN-Labs/nda-abcd-s3-downloader)
* [Download ABCD derivatives](https://collection3165.readthedocs.io/en/stable/)

### Data on Openmind
* Phenotypic/Behavioral data are stored on OpenMind at `/om2/user/maedbh/abcd_data/ABCD4`
