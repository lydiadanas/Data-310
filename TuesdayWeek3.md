We used data from the iris dataset in our model. It measures sepal length, sepal width, petal length, and petal width for three species of flowers.

To create a tf.dataset, we first used tf.keras.util.get_file to import the dataset from its url. Then we identified what column labels are features and what column label is the target, as well as the target’s class names. Finally, we used tf.data.experimental.make_csv_dataset to create a tf.dataset. 
We passed in the training dataset as the data, a 32 batch size, the column names as the feature names and the label name as the target name, and set the number of epochs to 1. 
This function then shuffled/parsed through the data and reorganized it into a tf.dataset, which is characterized by dictionaries where feature names are the key and numbers are values. In other words, the columns are individual dictionaries, which makes them mutable and iterable. Also, the amount of values that are displayed in the arrays were controlled by the batch size of 32.

