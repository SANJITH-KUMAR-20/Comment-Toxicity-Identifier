# Comment-Toxicity-Identifier
A Gradio App that categorizes the toxicities in a comment using NLP

The dataset for this model is from kaggle competition- https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge

We load in the data and preprocess it for prediction
    
    1. Load in the data and use the TextVectorization layer in tensorflow(tf.keras.layers.TextVectorization)
    2. Load the data and labels as tf.Dataset object
    3. cache, shuffle, batch and prefetch the data
    4. Split into train,test and validation sets

Build the model:
    
    1. Build a bidirectional LSTM model.
    2. Use BinaryCrosentropy loss to predict for different output parameters
    3. Use adam optimizer for optimization
    4. Train the model and tune the hyperparameters for better results
    
Gradio app:
    
    1. Use the gradio module to create the gradio application which helps with deployment.
    2. Create an interface object with necessary parameters and launch the application.
    
    
