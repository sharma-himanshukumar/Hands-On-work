# Convolutional Neural Network
The idea is to create a Neural Network that can detect if the image is a rectangle or a Circle. The training data is present in the input file, data-set is created on paint one by one (Yes I sound very idiotic I can understand, based on my curiosity).

The Convolutional Network data is just based on own judgement if you Fork it feel free to change the model.


Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_6 (Conv2D)            (None, 224, 224, 32)      896       
_________________________________________________________________
conv2d_7 (Conv2D)            (None, 222, 222, 32)      9248      
_________________________________________________________________
max_pooling2d_3 (MaxPooling2 (None, 111, 111, 32)      0         
_________________________________________________________________
dropout_4 (Dropout)          (None, 111, 111, 32)      0         
_________________________________________________________________
conv2d_8 (Conv2D)            (None, 111, 111, 64)      18496     
_________________________________________________________________
conv2d_9 (Conv2D)            (None, 109, 109, 64)      36928     
_________________________________________________________________
max_pooling2d_4 (MaxPooling2 (None, 54, 54, 64)        0         
_________________________________________________________________
dropout_5 (Dropout)          (None, 54, 54, 64)        0         
_________________________________________________________________
conv2d_10 (Conv2D)           (None, 54, 54, 64)        36928     
_________________________________________________________________
conv2d_11 (Conv2D)           (None, 52, 52, 64)        36928     
_________________________________________________________________
max_pooling2d_5 (MaxPooling2 (None, 26, 26, 64)        0         
_________________________________________________________________
dropout_6 (Dropout)          (None, 26, 26, 64)        0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 43264)             0         
_________________________________________________________________
dense_1 (Dense)              (None, 512)               22151680  
_________________________________________________________________
dropout_7 (Dropout)          (None, 512)               0         
_________________________________________________________________
dense_2 (Dense)              (None, 2)                 1026      
=================================================================
Total params: 22,292,130
Trainable params: 22,292,130
Non-trainable params: 0
_________________________________________________________________
