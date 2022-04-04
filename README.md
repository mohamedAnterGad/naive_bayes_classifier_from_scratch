# naive_bayes_classifier_from_scratch
here is the implementation of naive bayes from scratch on python using pandas, numpy and math libraries

could you ever imagined that a naive assumption will result in a very good practice results??
well here is the naive bayes clssifier that perform very good even knowing it's built on a naive assumption

the naiive assumption is that :
    1. all the features entering the model are independent features
    2. the distribution of the feature is of normal distribution (can assume any other distribution according to the metadata of the features)
the naive bayes classifier is based on a simple rule in mathematics which is the following equation:

![image](https://user-images.githubusercontent.com/47314651/161601186-ece3520a-1d9b-4ad4-97bb-0b3ac83aa9ee.png)

the evidence is the probability of the features
the liklihood is the probability of having the class given the features
the prior probability is the prior assumption about the probability of the classes

the naive doesn't compute the denominator as it's the same in all the classes 
given the numenator for all the classes it compares them and takes the largest number as the prediction


## my implementation :
1. my model works only on the numeric input data 
2. can work on a categorical target data (classes to predict)
3. works on multi features and multi class output
4. makes an assumption that all the features are of normal distribution
5. doesn't check for numeric columns so if you entered a categorical one you will encounter an error


## how to use:
1. just make an object of the class Bayes and pass to it the training data(including the labels) and the name of the target_column
2. call the method calc_naiive_bayes which takes parameters: (this is the predict function)
   the x_test 
   features_names : optional parameters represents the name of the features to use to predict the class
   x_test : data frame containing the test data
   distribution : default normal (no other distribution available)
 returns two lists :
      1. output predicted classes
      2. output probability for the predicted class
