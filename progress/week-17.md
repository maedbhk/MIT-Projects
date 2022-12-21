---
title: Week 17
---

* Worked on adaptive ADHD project with Alyson + Lexi, specifically getting data from UK Biobank on professions.
    * not all of the data is on openmind so we've been requesting certain variables from UK Biobank (e.g., psychiatric diagnoses)
* Alyson has become interested in better understanding girls with ADHD and how their cognitive profiles are different from boys with ADHD. It's an under-researched topic in the literature, and we have found some differences in the HBN dataset between girls and boys with ADHD. Some topics we discussed:
    * Babinski (2019): Sex + Puberty Moderate Association Between ADHD and Depression
    * Dir (2019): Pubertal influences on neural activation during risky decision-making in ADHD
    * Ostojic (2016): Association Between Pubertal Onset and ADHD Symptoms
    * Camara (2020): Relationship Between Sex Hormones, Reproductive Stages, and ADHD
    * Hamlat (2019): Pubertal Timing as Transdiagnostic Risk for Psychopathology
    * Halkett (2021): Initial Engagement in Oral Sex/Intercourse in Girls with and without ADHD
    * Why are girls in the inattentive ADHD subtype diagnosed later than boys?
    * Are there more ADHD subtypes beyond combined/hyperactive/inattentive?
* Wrote a script to run SUIT (and SUITPy) on anatomical scans from HBN. Putting the derivatives from SUIT into a similar format as adopted in this [functional fusion](https://github.com/DiedrichsenLab/Functional_Fusion) project
    * SUIT has to run on the fmriprep derivatives and fmriprep hasn't been run yet on all HBN participants. I've tested the script out on a subset of participants that Jeff processed with fmriprep
* Worked with Shreya on predictive modeling pipeline, spent some time figuring out imbalanced train and test sets, and multi-label classification