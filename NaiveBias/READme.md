Naive Bayes :
- The naive bayes classifer learns by by assuming features are independent for a given class so it is conditonally independent.
- Its foundation is from the Bayes's theorem which is :
  P(A / B) = P(B /A ) * P(A) /P(B)
  where P(A /B) is called the posterior probability
        P(B/A)=likelihood
        P(A) - prior prbability
        P(B) -evidence.
  - for classification:  P( class / X) = P(X/class) * P(class)  / P(X)
                       where X=(x1,x2,x3,x4......xn) these are the features
  - So when any Zero Probabilities occure then we perform Laplace Smoothing. 
  - As P(X) is constant for all the classes so we can say that P(class /X) is directly proportional to P(X/class)* P(Class).
  - So the laplace smoothing works like this:
        P(X/class) = Count of xi in class  + 1   / Total in class + # possible values      (possible values = total values in class).
-Types of Naive bayes:
1. Gaussian Naive Bayes- to follow the gaussian (nominal) ditribution.
   ![image](https://github.com/user-attachments/assets/947096dc-2a58-4d86-a9e3-89f02ba44d31)

3. Multinomial Naive Bayes- for discrete data.
4. Bernoulli Naive Bayes- for binary and boolean data.
    
- Ex:This can be used for the text classification(spam detection and sentiment analysis),medical diagnosis and system performance management,bioinformatics(for classifying gene expression data),Anamaly detection(for indentifying outliers in datasets)
