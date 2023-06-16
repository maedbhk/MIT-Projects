---
title: Exploring ADHD in children and adolescents (leveraging the healthy brain network dataset)
---

## Research Qusetions
* **Some of these questions have been addressed [here](../notebooks/exploratory-features-adhd.ipynb)**
* What % of children with adhd have parents with adhd? `PreInt_FamHx,m_adhd` `PreInt_FamHx,f_adhd`
*  What is the SES/race/gender breakdown of children with adhd? 
* What are the kinds of professions / college education held by parents of kids with adhd?
* School environment for children with adhd `PhenX_School`
* Neighborhood environment for children with adhd `PhenX_Neighborhood`
* How do general scores of achievement and intelligence differ across adhd subtypes? 
* What is the gender breakdown of adhd subtypes? 
* Girls with adhd: 
    * age of first menstruation 
    * age of puberty onset
* what kind of school organizations are kids with adhd part of? `PreInt_EduHx`
* Family history of mental illness `PreInt_FamHx` or other illness
    * primary diagnosis of mother, father, sibling
* What % of children are taking medication for adhd? 
* What type of allergies do children with adhd have?
* Previous head injuries? 
* Mother's nicotine use during pregnancy?
* Severity of ADHD diagnosis - differences across subtypes (inattentive, hyperactive etc.)
* Any information on whether people with adhd are night owls versus early risers?
* Any difference in rates of suspension, detention in children with ADHD compared to children without a diagnosis? 
* Is there any evidence that children with ADHD spend longer on the internet than children without adhd, and what is the nature of internet usage?

## Questions - Child Behavior Checklist - Teacher Report Form
* What information is captured in this questionnaire? 
    * teacher / parent differences in CBCL in girls with ADHD - difference in reporting?
    * what scales you use to diagnose ADHD result in different subtypes

## Questions - Predictive modeling
* ADHD: can subtypes be classified from one another?
    * hypothesis: most questionnaires/measures will not be able to differentiate between adhd subtypes
* ADHD: can gender be classified from one another?
    * hypothesis: certain questionnaires will be able to identify between gender
* are there boys/girls who have cognitive profiles similar to those with adhd but haven't been diagnosed with adhd?
    * how do we address this question? determine a cognitive profile for each participant and do a similarity comparison between those diagnosed with adhd and those without, are there any participants who have a cognitive profile that is very similar to ADHD but were not given a diagnosis?

## Summary of cognitive performance
* Many questionnaires (e.g., measures) have a `total` or `raw` score providing an overall summary of how well a participant did on a questionnaire
* For all of the measures that have a `total` or `raw` score, how well on average are children with ADHD (across subtypes and gender) performing on these assessments compared to children without a diagnosis?
