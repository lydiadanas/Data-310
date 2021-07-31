1. Generated text:
   

2. How it was produced:
   
    a. Processing, vectorizing and predicting text
        
   To vectorize the text, we first split the text into tokens with tf.unicode_split, then used preprocessing.StringLookup
        to vectorize the characters.To predict text, we trained the model to predict the next most likely character, and used
        .StringLookup with invert = True as well as tf.reduce_join to first convert the predicted numbers back to characters, and 
        then join the characters back into words.
   
    b. Building and training the model
        
    To build the model, we created a model subclass with one embedding layer, a gated recurrent unit layer, and a dense output layer.
    Before training, we set the loss function to SparseCategoricalCrossentropy, set the optimizer to adam, and compiled the model.
    Then we made sure to save training checkpoints, and ran the model.
    
    c. Generating text
   