# Sem6_NLP_Project
Multi-label multi-class classification(tag prediction) of Stack Overflow questions along with Topic Modelling. Tag prediction model is deployed locally and users can enter their questions in the Streamlit web app and get the predicted tags. Two approaches have been tried here, **supervised** - through the classification model and **unsupervised** through topic modelling.

**Supervised approach -**
Different base classifiers were tried for the tag prediction model - **Logistic Regression**, **Decision Trees**, **SGDClassifier** and different wrappers over these simple classifiers(that do not natively support multi-target classification) - **MultiOutputClassifier**, **BinaryRelevance**, **ClassifierChain**, **LabelPowerset**, etc. 

**Unsupervised approach -**
In topic modelling, Latent Dirichlet Allocation (LDA) models have been used - LDA & LDAMulticore . Coherence Model has been used to evaluate how distinct and separable the generated topics are for each LDA model .

Both the approaches can be used and compared. Either one of them can be used finally or better, both can be used together. The predicted tags can be used to filter the topics and the user can get a more descriptive tag, so like instead of just **python** tag getting predicted something like **python - TypeError** would be more helpful. 

