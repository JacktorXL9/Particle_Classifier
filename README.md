# Particle_Classifier
A simple classifier for particles detected based on GEANT simulated data. The data set for the repository is too large to be uploaded to github so it can be found here https://www.kaggle.com/naharrison/particle-identification-from-detector-responses.
There were a fair amount of problems when dealing with this data set first and foremost being that several of the columns are not useable as they have a vast majority of their data points as zero.
Secondly the data is greatyl skewed in the respect that there are far fewer points for two of the targets than the other two.
However despite all this I was able to make a fairly simple classifier using the RandomForest method that predicted the values of the larger targets to  precision >= 97% and the smaller targets to precisions >=75% which I feel is quite solid given the issues.
I will be exploring other methods with this data in the future and will post what updates I make here.

Note: I am presently having difficulties getting the jupyter notebook to open and this seems to be a fairly common issue. A full rendering of the notebook can be found here
https://nbviewer.jupyter.org/github/JacktorXL9/Particle_Classifier/blob/master/Particle_Classifier.ipynb

Version 1.0 2019-03-27
Base

Version 1.0.1 2019-03-29
Added a link to a notebook viewer as GitHub's seems unstable

Version 1.1 2019-04-03
Worked with a more biased data set which had an equal distribution of the 4 targets. This produced much better results for the positrons and the kaeons but hurt the accuracy of the other two variables. In addition to this and XGBoost classifer was used to see if any imporvements could be made however it did not perform any better than a RandomForestClassifier. In addition to this a model was built using the entire data set, but due to the lack of the afformentioned biasing towards the less represented variables, not much improvement was made.
