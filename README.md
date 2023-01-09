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
- For Int Values Using Simple Imputer From sklearn with stratergy = "mean.
- Dropping "id" as it is not that necessary
- Then converting all the string value into int by using Label Encoder from sklearn
