# Measuring-Campaign-Effectiveness
Using machine learning to predict which customers are more likely to respond to bank’s marketing campaigns?

## Data Set Information:

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. 
Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. 
The dataset consists of 45211 observations and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]


## Objective

The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).


## Attribute Information:

### Input variables:
#### bank client data:
<br/>1 - age (numeric)
<br/>2 - job : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
<br/>3 - marital : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
<br/>4 - education (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
<br/>5 - default: has credit in default? (categorical: 'no','yes','unknown')
<br/>6 - housing: has housing loan? (categorical: 'no','yes','unknown')
<br/>7 - loan: has personal loan? (categorical: 'no','yes','unknown')
#### related with the last contact of the current campaign:
<br/>8 - contact: contact communication type (categorical: 'cellular','telephone') 
<br/>9 - month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
<br/>10 - day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
<br/>11 - duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
#### other attributes:
<br/>12 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
<br/>13 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
<br/>14 - previous: number of contacts performed before this campaign and for this client (numeric)
<br/>15 - poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')
#### social and economic context attributes
<br/>16 - emp.var.rate: employment variation rate - quarterly indicator (numeric)
<br/>17 - cons.price.idx: consumer price index - monthly indicator (numeric) 
<br/>18 - cons.conf.idx: consumer confidence index - monthly indicator (numeric) 
<br/>19 - euribor3m: euribor 3 month rate - daily indicator (numeric)
<br/>20 - nr.employed: number of employees - quarterly indicator (numeric)

### Output variable (desired target):
<br/>21 - y - has the client subscribed a term deposit? (binary: 'yes','no')

### The final report with findings can be found [here](http://rpubs.com/nitishghosal/370759).
