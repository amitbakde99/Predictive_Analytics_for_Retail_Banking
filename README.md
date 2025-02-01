# Predictive Analytics for Retail Banking

## Objectives of Research

Analytics is helping the banking industry become smarter in managing the myriad challenges. Challenges:

* What is a suitable product to recommend to a customer?
* What is the best time to market the product?
* Which is the most effective channel to contact a customer?

The data is related with direct marketing campaigns of a banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. The goal is to predict if the client will subscribe a term deposit.

## Problem Statement

The data-set is related with direct marketing campaigns (were based on phone calls) of a banking institution. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. The goal is to predict if the client will subscribe a term deposit.


## Columns:

* age : Age of the client- (numeric)
* job : Client’s occupation - (categorical) (admin, blue-collar, entrepreneur, housemaid, management, retired, self employed, services, student, technician, unemployed, unknown)
* marital : Client’s marital status - (categorical) (divorced, married, single, unknown, note: divorced means divorced or widowed)
* education : Client’s education level - (categorical)
* default : Indicates if the client has credit in default - (categorical) (no, yes)
* balance : average yearly balance, in euros (numeric).
* housing : Does the client as a housing loan? - (categorical) (no, yes)
* loan : Does the client as a personal loan? - (categorical) (no, yes)
* contact : Type of communication contact - (categorical) (unknown, cellular, telephone)
* day : Day of last contact with client.
* month : Month of last contact with client - (categorical) (Jan - Dec)
* duration : Duration of last contact with client, in seconds - (numeric)For benchmark purposes only, and not reliable for predictive modelling.
* campaign : number of contacts performed during this campaign and for this client (numeric, includes last contact) - (numeric)(includes last contact)
* pdays : Number of days passed  client was last contacted - (numeric)(-1 means client was not previously contacted)
* previous : Number of client contacts performed before this campaign - (numeric)
* poutcome : Previous marketing campaign outcome - (categorical)
* deposit: field used to split the data into two sets (client has deposited, or not)


## Conclusion

Most classification problems in the real world are imbalanced. Also, almost always data sets have missing values. In this post, we covered strategies to deal with both missing values and imbalanced data sets. We also explored different ways of building ensembles in sklearn. Below are some takeaway points:

* Sometimes we may be willing to give up some improvement to the model if that would increase the complexity much more than the percentage change in the improvement to the evaluation metrics.
* When building ensemble models, try to use good models that are as different as possible to reduce correlation between the base learners. We could’ve enhanced our stacked ensemble model by adding Dense Neural Network and some other kind of base learners as well as adding more layers to the stacked model.
* Easy Ensemble usually performs better than any other resampling methods.
