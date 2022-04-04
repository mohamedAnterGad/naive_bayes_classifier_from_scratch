# naive_bayes_classifier_from_scratch
here is the implementation of naive bayes from scratch on python using pandas, numpy and math libraries

could you ever imagined that a naive assumption will result in a very good practice results??
well here is the naive bayes clssifier that perform very good even knowing it's built on a naive assumption

the naiive assumption is that all the features entering the model are independent features
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
4. doesn't check for numeric columns so if you entered a categorical one you will encounter an error

