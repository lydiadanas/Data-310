1. Predicting wealth vs all other classes as binary target

    - Best model:
      My best model was my fifth model. In my second model, I adjusted bucket sizes by using np.percentile to calculate the 25, 50, and 75th percentiles for the age and size columns.
      I changed my age buckets from 9, 18, and 75 to 7, 16, and 35. 
      Then in my fifth model, I removed the car column because it had very little variation in value. This slightly improved the accuracy of my model, but it mostly evened out the variation between accuracies for each epoch.
      Overall, every model I tried only resulted in small changes to the accuracy, and because of this my graphs all look very similar.
      ![img_53.png](img_53.png)
    - Worst model:
      My worst model was my first model.
      I used a numerical size column, a bucketized age column, and made the rest of the columns categorical. This was using Wednesday's approach. What was interesting about not only this model but the other models was that the worst accuracy was on the second wealth class, not the first.
      ![img_54.png](img_54.png)
    
2. Confusion matrix

First model:
![img_57.png](img_57.png)
![img_58.png](img_58.png)

Second model:
![img_55.png](img_55.png)
![img_56.png](img_56.png)

   - Analyze and discuss two sets of results
      As you can see, there is very little difference between the two models and their accuracy.
3. Predicting wealth vs all other classes as categorical

    - Analyze and discuss results with confusion matrix as reference
    - Modify feature columns in attempt to improve accuracy with all 5 categorical wealth classes as target. Analyze and discuss progress and results.
    
    