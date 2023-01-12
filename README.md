# BikeBuyer
It is a classification data in which we try to predict if they will the bikes or not depending upon their
1. marital status,
2. Gender
3. Yearly Income
4. Children
5. Education
6. Occupation
7. Home ownership
8. cars
9. commute distance
10. Region
11. Age
- Analysing the data (EDA)
  - Check for NaN for in the dataset.
- For String values filling the NaN values by using fillna methods.
- For Int Values Using Simple Imputer From sklearn with stratergy = "mean".
- Dropping "id" as it is not that necessary
- Then converting all the string value into int by using Label Encoder from sklearn
- For preprocessing we use Binarization as it only consider the presences or absence of a feature rather than a quntified number of occurences for instances
- Now we start applying algorithms 
   1. DecisionTreeClassifier  **(89.98)**
   2. KNeighborClassifier **(89.006)**
   3. LogisticRegression **(89.91)**
   4. SVC **(89.918)**
   5. GaussianNB **(89.26)**
   4. LinearDiscriminantAnalysis **(89.918)**
       - for scoring we use "accuracy"
       - for model_selection we use ShuffleSplit(n_splits = 10,test_size = 0.33,random_state = 8)
- To visualise the comparison we plot the data in boxplot form.
- By using pipeline we first preprocess the data using standardscaler and than applied all the classification algorithms
   - In which we find that svc has the best accuracy of **89.99**
- We again try to find the best kernels among "linear","poly","rbf","sigmoid"
  - find out that with kernel = "poly" show the best accuracy of **90.1**
- We again apply all ensembles algorithms just to check if there is any better accuracy but there wasnnot 
- We consider SVC (poly) as the final model
