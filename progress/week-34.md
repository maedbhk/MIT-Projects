---
title: Week 34
---

04/10/23 - 04/14/23

## Done and To Do
* Presented in lab meeting, presentation [here](https://docs.google.com/presentation/d/1rF-d7UbZxG15-XzZE4iVqKMK9k_lCTrprmX-r3Colcg/edit?usp=sharing)
* Interviewed more RAs to work on the NLP + HBN project
    * Hoping to have someone take over this project during the summer
* Updated dataset info for [ABCD](../datasets/abcd.md), [healthy brains](../datasets/healthy-brains.md) and [uk biobank](../datasets/uk-biobank.md) datasets
    * trying to keep track of which data are where, would be great to have this as part of a lab wiki that people update frequently
* A subset of [fMRIPrep](https://fmriprep.org/en/stable/) + [XCP](https://xcp-d.readthedocs.io/en/latest/) derivatives for HBN are now on OpenMind at `/nese/mit/group/sig/projects/hbn/hbn_bids/derivatives` (thanks to Steven Meisler)
* Working with Steven to process the entire HBN dataset (fmriprep + xcp pipeline)
* Updated phenotypic data for ABCD, currently at `/om2/user/maedbh/abcd_data/ABCD4` (will move to nese at some point)
* UKBiobank phenotypic data have also been updated at `/om2/user/maedbh/ukbiobank_data` (will move to nese at some point)
* Having lots of difficulty running HBN models on OpenMind this week - don't think it's an issue with the nodes rather something to do with pydra-ml, scripts are running but hanging on the `gen_workflow` function (no idea why) - have spent lots of time troubleshooting
    * shreya is having similar difficulty with the developer distrubtion of pydra-ml in trying to implement multi-label classification
* example of suit derivatives is on OpenMind here: 
* played around with [cerebellar transcriptomic data](https://cellxgene.cziscience.com/e/095940cb-7422-4510-96e2-cbafd961eb88.cxg/) - need to think more about specific questions