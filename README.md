# Cell Segmentation

### Built With

* Tensorflow
* Keras 

### Data

The original dataset is from [isbi challenge](http://brainiac2.mit.edu/isbi_challenge/)
The data for training contains 30 512*512 images,

**Data augmentation** : ImageDataGenerator in keras.preprocessing.image 

Output from the network is a 512*512 which represents mask that should be learned. Sigmoid activation function makes sure that mask pixels are in [0, 1] range.

### Training
The model is trained for 5 epochs.

Accuracy ~ 0.97.

Training loss function - binary crossentropy.

## Results
Trained model to do segmentation on test images

![img/0test.png](img/0test.png)

![img/0label.png](img/0label.png)