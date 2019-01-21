# Movie-Reviews-Classification
Binary Sentiment Analysis on movie reviews

We have replicated the features that were used in the original paper. A movie review is featurized as a bag-of-words, where each feature is the number of times a particular word occurs in the review. Of course, most words don't occur in a single review. So while the dimensionality of the feature vector is the number of words (in this case 74481), most reviews correspond to very sparse vectors in this space.

Classifiers implemented from scratch include:
* [Margin Perceptron](https://nbviewer.jupyter.org/github/TarunSunkaraneni/Movie-Reviews-Classification/blob/master/margin-perceptron-movie-review-classifier.ipynb): accuracy of 87.3% on testing data, 87% on validation data
* [Average Perceptron](https://nbviewer.jupyter.org/github/TarunSunkaraneni/Movie-Reviews-Classification/blob/master/average-perceptron-movie-review-classifier.ipynb): accuracy of 87.6% on testing data, 88.4% on validation data
* [SVM](https://nbviewer.jupyter.org/github/TarunSunkaraneni/Movie-Reviews-Classification/blob/master/svm-classifier.ipynb): accuracy of 88.89% on testing data, 88.2% on validation data
* [Logistic Regression](https://nbviewer.jupyter.org/github/TarunSunkaraneni/Movie-Reviews-Classification/blob/master/logistic-regression-movie-review-classifier.ipynb): accuracy of 86.8% on testing data, 86.9% on validation data
* [Naive Bayes](https://nbviewer.jupyter.org/github/TarunSunkaraneni/Movie-Reviews-Classification/blob/master/naive-bayes-movie-review-classifier.ipynb): assumes a Gaussian data distribution, accuracy of 81.6% on testing data, 80.8% on validation data
* [Neural Network](https://nbviewer.jupyter.org/github/TarunSunkaraneni/Movie-Reviews-Classification/blob/master/neural-net-movie-review-classifier.ipynb): accuracy of 86.3% on testing data, 86.2% on validation data

All classifiers are compliant with Scikit-learn's API, and that makes it possible to use Sklearn's CV and Gridsearch functions. This allows for multi-core training and cross-validation capability. 
