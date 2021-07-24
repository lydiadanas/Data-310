Unfortunately I was having issues with my model.fit call on Wednesday night, so I was unable to work with Michael and Dylan. Once I got it working on Friday afternoon, I tried to make a better model than they did but found their buckets and structure resulted in the highest accuracies, especially when looking at the highest wealth.

I made the plot below comparing my intial accuracy and the accuracy with Michael and Dylan's model:

![img_44.png](img_44.png)

My first model:

- Numeric columns - size, age

- Indicator columns - gender

- Categorical columns - edu

- No crosses



Michael and Dylan's:

- Numeric columns - size

- Bucketized columns - age

- Indicator columns - gender, edu

- Crosses - age and size