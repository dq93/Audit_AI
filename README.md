# ML_financial_fraud

You are a data scientist working for a NYC-based international bank called Caishen. After the winter break, the company announced in an all-hands meeting that the goal for the next 3 years will be to identify fraudulent activity within their customer-facing bank accounts. While your cybersecurity team has provided you with a dataset of historic fraudulent activity, the responsibility of designing a minimal-viable-product (MVP) has fallen on your desk. 

For this project you will be creating an ensemble classifier (random forest or boosted model) that will assess if fraudulent activity has occurred for a transaction. Download the dataset from the following link: https://drive.google.com/file/d/1udzVidq-uKp-muCJ0ZReHJ5mjCafesuE/view?usp=sharing Links to an external site.

# Report
i. I saw that there is not there is little correlation between the features and that this dataset is very imbalanced, making some of these model like KNN, not good candidates for this.

ii. I dropped step because time doesn't seem to correlate with fraud or anything really, nameOrigin and nameDest because the account's name don't make a difference since they appear to be generated in a way that doesn't make sense to a human reading it, and isFlaggedFraud because this feature simply marks any transaction over 200K as possible fraud.

iii. I only used the default hyperparameters.

iv. I'd say the performence improved for all even if the accuracy dropped, because they missed less cases of fraud.

v. My final f1 score was for logarithmic regression was .33, for naive bayes it was 0.0040, and for KNN it was 0.3381.