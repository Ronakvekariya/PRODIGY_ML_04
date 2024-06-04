# Hand Gesture recognistion system  :
- Hand gesture recognition is a technology that interprets human hand movements using various sensing devices.
- This system can be employed in diverse applications such as human-computer interaction, sign language interpretation, virtual reality, robotics control, and gaming.

  
# DataSet :
Dataset Link

# Data Preparation
The image data needs to be prepare as per the need of the model.
For the svm , The image data is store as array as Grayscale images.
And the data is resized (reduce) to efficiently load and use the image by CPU and GPU

# Model :
  1. Layer 1 :- 32 fiter , kernel size = 3*3 , activation function = RELU , BatchNormalization , MaxPooling = 2*2 , Dropout = 20%
  2. later 2 :- 65 fiter , kernel size = 4*4 , activation function = RELU , BatchNormalization , MaxPooling = 2*2 , Dropout = 30%
  3. layer 3 :- Flattern
  4. layer 4:- Dense , 1024 neuron , activation function = RELU , Dropout = 50%
  5. layer 5 (OutPut layer):- Dense , 10 neuron , activation function = SOftMax

# Model Parameter :-
- optimizer :- RMSProp
-  loss = 'categorical_crossentropy'
-  metrics = 'accuracy'
  
# Regularzation :-
  - Regularization techniques impose constraints on the model to simplify it and improve its generalization performance.
  - For this application the following effective technique has used
      1. Dropout
      2. Early Stopping

# Training :-
   - Model is train for 10 epochs

# Result:-
- accuaracy :- 0.9999
