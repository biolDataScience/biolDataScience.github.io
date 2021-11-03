
### Breiman 'two cultures'

`Prediction` To be able to predict what the responses are going to be to future input variables; 

> Algorithmic modeling culture: the shape of that function(x) of the predictor variables is unknown, and we shouldn't specify a form. Focus is on model validation by predictive accuracy. 



`Information` To extract some information about how nature is associating the response variables to the input variables

> Data modeling culture: values of parameters are estimated from data, assuming that there is some known function that links predictor and responses, where information is the main goal.





1) Focus on finding a good solution-that's what consultants get paid for. 
2) Live with the data before you plunge into modeling. 
3) Search for a model that gives a good solution, either algorithmic or data. 
4) Predictive accuracy on test sets is the criterion for how good the model is. 
5) Computers are an indispensable partner. 




Rashomon: the multiplicity of good models; 
Occam: the conflict between simplicity and accuracy; 
Bellman: dimensionality-curse or blessing



#### Questions for discussion:

What are the two cultures of statistical modeling? 

(data modeling and algorithmic modeling)


What role do you think consulting had in changing Breiman's view of statistical modeling? How did the consulting problems fundamentally differ from typical academic problems?

(ozone example, the focus was inherently on prediction (nearly real-time) and the feature set was huge; most of the projects listed on page 200 deal with predictive modeling and not inference)




What are the benefits of having an explicit data model (i.e., assuming that the data are generated according to some pre-set model)?




What issues are discussed in the context of the linear regression example in 5.1, and more generally in section 5?






What are some limitations of data models, and how have the lines been a bit blurred in more recent years?





If Breiman were to re-write section 7.1 of this paper, what do you think would be the same/different?

(deep learning and the huge advent of statistical learning would definitely be discussed at length) 




How does Breiman define model "instability" and the multiplicity problem? Have you encountered something similar to this yet? What is Breiman's proposal for one solution to this problem? 

(model error is same but variable sets and model structure can be quite different. Selecting only the most relevant predictors necessitates that such a clean subset exist, which is rarely the case. Bagged trees and algorithmic approaches which can account for an expanded number of covariates can be stable and yield good performance. This can also exist in a data modeling approach though too, which blurs the lines, as L1/regularized regression is essentially a data-modeling way to still assume a functional form, but to allow coefficients to shrink to 0 effect. )





What is the conflict between prediction, accuracy, and simplicity that Breiman discusses in reference to Occam's razor/dilemma?  

(Accuracy generally requires more complex prediction methods. Simple and interpretable functions do not make the most accurate predictor)






What is the curse of dimensionality? Why is it maybe not so much a curse? When is it not so much a curse?

(a side note: the NIST dataset still exists and the challenge is still a useful one for exploring how to classify simple images. https://www.kaggle.com/c/digit-recognizer)










In section 11, Breiman gives a neat example about variable importance and model selection. What are the differences in approach from the logistic regression and variable importance estimation relative to the random forest and variable importance estimation procedure there?

(logistic regression followed by bootstrapped model fits found top n variables in the best fit model were only in the submodels like 60% of the time. Random forest found a consistent effect of two variables, both of which were collinear and explained pretty much the same proportion of variance in the test set.)







How do we assess model performance generally?

(R2, p-values, predictive accuracy. be sure to mention train/test split and the issue of class imbalance). 








What were your major takeaways from this paper?





