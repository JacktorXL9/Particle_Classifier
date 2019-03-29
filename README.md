# Particle_Classifier
A simple classifier for particles detected based on GEANT simulated data. The data set for the repository is too large to be uploaded to github so it can be found here https://www.kaggle.com/naharrison/particle-identification-from-detector-responses.
There were a fair amount of problems when dealing with this data set first and foremost being that several of the columns are not useable as they have a vast majority of their data points as zero.
Secondly the data is greatyl skewed in the respect that there are far fewer points for two of the targets than the other two.
However despite all this I was able to make a fairly simple classifier using the RandomForest method that predicted the values of the larger targets to  precision >= 97% and the smaller targets to precisions >=75% which I feel is quite solid given the issues.
I will be exploring other methods with this data in the future and will post what updates I make here.

Version 1.0 2019-03-27
Base

  $jupyter nbconvert --to html Particle_Classifier.ipynb
