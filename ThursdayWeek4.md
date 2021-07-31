1. Generated text:
   
   ROMEO:
   
   Tybalt, hasty and all my lands,
   
   I am his word 'brothecy, take up my books,
   
   He loved his brother's pains: she bring his state
   
   He had a baby fair lime and down.
   
   QUEEN:
   
   And 'twas to jest.

   GLOUCESTER:
   
   Your grace seal'd me to-day; for thou hast broke
   
   To be proud wind that blows you hopest.
   
   KING HENRY VI:
   
   And far I brother, did my stay with sills,
   
   And bown before him to the Tower,
   
   My friends ado, with splander of my state,
   
   And presently as we may grate lunar.
   
   Alas, I fay, it will not slept; and see who shakels,
   
   But in the lessen chose ignorance
   
   To fair for what my sister learns.
   
   DUKE OF YORK:
   
   I'll not believe it; I'ld not live like givence:
   
   My pares after 'tis enough to proud, Juliet.
   
   PRINCE EDWARD:
   
   Richard you have been tongued. How now! what news?
   
   BUCKINGHAM:
   
   Well, sir, nor form and grandsire strong on't.
   
   DUKE VINCENTIO:
   
   There let me lie in circu.
   
   ANTONIO:
   
   Of stronger of men, no beyond;
   
   Then whet me dissentious rumedless death,
   
   But what to shame us wretch,
   
   Do whist not half; which


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
   
   To generate text, we defined a one step model class that we then ran in a loop.