1. Describe the dataset

    - Type of variable (target): binary
    - How many features are being used: 28
    - How many observations are in the training dataset: 10,000
    - How many are used in the validation set: 1,000
    

2. Performance
![img_8.png](img_8.png)
    - How did each of the models perform?
      
      The tiny and small models performed the best, but the medium and large models did not perform well at all.
   
    - Which of the four performed the best?
   
      The tiny model performed the best.
    - Which ones performed the worst?
      
      The medium and large models performed the worst.
![img_9.png](img_9.png)
    - Why did some perform better?
      
      The ones that perfomed better were not overfit like the medium and large models were;
      while the dataset itself is large, there are only 28 features and the larger network sizes 
      that lead to overfitting were all over 28 units and the smaller ones were all under 28 units, so that could have something to do with it.
    

3. Overfit

    - What is an overfit model?
      
      An overfit model is a model with higher capacity than the dataset.
    - Why is it important to address it?
      
      Overfit models will not be able to generalize their predictions accurately.
    - What are four ways we have addressed it so far?
      1. Decreasing the size/complexity of the model in general (not by weights)
      2. L2 regularization 
      3. Dropout
      4. Combined L2 and dropout
    

4. Load and preprocess images

    - What are you functionally accomplishing as you apply the filter to your original array?
    - Why is the application of a convolving filter to an image useful for computer vision?

   - In effect what have you accomplished by applying this filter?
   - Does there seem to be a logic (i.e. maximizing, averaging or minimizing values?) associated with the pooling filter provided in the example exercise (convolutions & pooling)?
   - Did the resulting image increase in size or decrease?
   - Why would this method be useful?
   

5. Matrix:
