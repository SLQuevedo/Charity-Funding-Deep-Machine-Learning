# Charity-Funding-Deep-Machine-Learning

# Preprocessing
First I determined that our target variable is the successfulness of the applicaiton. I dropped the 'Name' and 'EIN' because I determined that they would not be useful for this model. The feature vaiables were application type, affiliation, classification, use case, organization, status, income amount, special considerations and ask amount. I binned uncommon application types to create a new "other" application type. I binned the classification types with a count of less than 1800 into the "other" classification type. I converted the categorical data into numeric values and then scale my data. 

# Compiling and Training
In my first optimization I used 2 hidden layers and the relu and sigmoid activation functions. However, I was only able to achieve a 72.92% accuracy score with this method. With 100 epochs, I noticed that my model was fluxuating with its accuracy instead of leveling out. On my second optimization, I added an extra later and got an accuracy score of 72.99%. Once again my model was not leveling out. On my third attempt, I decided to use tanh and sigmoid activation functions with 4 layers and 50 epochs. I noticed that This had less variability than my previous models, but only yeilded an accuracy score of 72.90%. On my final attempt, I reduced the number of neurons to 6 for each layer and rebinned my application types. My model produced an accuracy score of 72.99% and had less variability with its predictions. 

# Results
I was unable to get the target accuracy score of 75%. More work is required to improve the accuracy of this model. 