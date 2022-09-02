---
title: Week 4
---

### Done
* Build [boilerplate ML pipeline](https://github.com/maedbhk/hbn_cerebellum) for building predictive models (tested so far on behavioral features from HBN)
* Cross-referenced pipeline with pydra-ml to determine that similar steps are being implemented
* Summary analysis on clinical diagnosis and demographics from HBN to determine adaquete sample sizes for cerebellar fingerprinting paper
* First pass using UMAP unsupervised learning on child measures (cognitive testing, physical fitness features etc.)
* Research on methods, focusing mostly on these three papers: 
    * GAMLSS modeling as used in [brain charting paper](https://www.nature.com/articles/s41586-022-04554-y)
    * LDA (topic modelling) as used in [endophenotyping of adhd paper](https://www.nature.com/articles/s41398-018-0179-6)
    * Brain age prediction as used in [brain age paper](https://www.nature.com/articles/s41593-019-0471-7) - gradient tree boosting

### To Do
* Try UMap in supervised mode to identify unique patterns in phenotypic data
* Questions to address: 
    * Within HBN assessment battery, which tests are most useful? (how does this vary across disorders?)
    * can further subtyping of individuals be done based on patterns in behavioral/cognitive assessments? (especially for 200 people who were not diagnosed due to an incomplete evaluation)
    * what is the reliability in the KSADS assessment across child and parent measures?
* Test python implementation of SUIT on subset (n=10) of hbn participants (T1w + T2)
* Perform VBM to measure local changes in structural abnormalities, following methods steps implemented in [this paper](https://www.sciencedirect.com/science/article/pii/S2213158218303012) - correcting for brain size etc.

### Questions:
* Don't yet have access to LORIS, will follow-up with Lindsay after labor day weekend
* CHOP Meeting - ask Satra to send email to folks there to set-up meeting sometime in Sep.? 
* Remind Satra to provide info about other project that we forgot to discuss in our 09/01 meeting
* I'm happy to be included in other projects (meetings etc.) if any seem like a good fit for my interests/skills
* Set up weekly meetings w/Satra on Wednesdays
* I would like to recruit 1-2 undergrad students through UROP - can I hire for pay or academic credit alone?
* I requested edit access to sign up for a lab meeting slot: I'm thinking either end of this month or beginning of oct. I guess the neuroimaging subgroup would be most appropriate but perhaps also knowledge engineering as the meeting will be soliciting feedback about project ideas. Let me know what you think.  