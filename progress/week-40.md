---
title: Week 40
---

05/22/23 - 05/26/23

## Done and To-Do
* Meeting with Ran and Elina on BHS data
* Mostly working ADHD Paper this week: methods + results
    * Model ABCD data (CBCL questionnaire)
    * Working with Elina to figure out how to identify ABCD participants with ADHD:
        * For ADHD we usually use the symptoms from:  abcd_ksad01 - ABCD Parent Diagnostic Interview for DSM-5 Full (KSADS-5)
        * To assess the severity of ADHD, we created an "or" variable for each symptom, considering both present and past occurrences, and then aggregated them [range 0-20]. 
        * A higher number of symptoms indicates a more severe ADHD condition. In some cases, we excluded the "Hyper" symptoms [range 0-10].
        * For the diagnosis, we also established an "or" variable. It is sufficient for an individual to have one of the four diagnoses listed below to meet the criteria for diagnosis.
![ADHD Symptoms](assets/images/adhd_symptoms_abcd.png){fig-align="center"}
