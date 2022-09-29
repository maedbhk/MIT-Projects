---
title: Model Interpretability
---

## Interpreting machine learning models
* intrinsic or post hoc? 
    * intrinsic: is interpretability achieved by restricting the complexity of the model. ML models are considered "intrinsically" interpretable due to their simple structure (short decision trees or sparse linear models)
    * posthoc: or by applying methods that analyze the model after training. ML models are considered "post hoc" models if they requir interpretation methods after model training. An example of such a model is permutation feature importance. Post hoc methods can be applied to intrinsically interpretable models. For example, permutation feature importance can be computed for decision trees. 
* counterfactual explanations: to explain the prediction of a data instance, the method finds a similar data point by changing some of the features for which the predicted outcome changes in a relevent way.
* intrinsically interpretable model: one solution to interpreting black box models is to approximate them (either globally or locally) with an interpretable model. the interpretable model is interpreted by looking at internal model parameters or feature summary statistics. 
* the interpretaton of regression weights in a linear model is a model-specific interpretation. by definition, the interpretation of intrinsically interpretable models is always model-specific. 
* model-agnostic tools can be used on any machine learning model an are applied after the model has been trained (post hoc).

## Scope of interpretability
* global model interpretablity helps to understand the distribution of target outcome based on the features (difficult to achieve in practice).
* any model that exceeds a handful of parameters or weights is unlikely to fit into the short-term memory of the average human. arguably, you cannot really imagine a linear model with 5 features - as it would mean drawing the estimated hyperplane mentally in a 5-dimensional space. any feature space with more than 3 dimensions is simply inconceivable for humans. 
* when people try to comprehend a model, they consider only parts of it, such as weights in linear models. 

### how do parts of the model affect predictions? 
* it's impossible to memorize all the weights (plus the joint distribution of all features) - but we can understand a single weight. global model interpretability is usually out of reach, but we can at least understand a single weight. 
* not all models are interpretable at a parameter level - for linear models, the interpretable parts are the weights, for trees it's the splists (selected features plus cut-off pointss), and leaf node predictions. 