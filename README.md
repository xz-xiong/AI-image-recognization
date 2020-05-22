# AI-image-recognization use Keras

This is a project from IBM AI course training program.

The jupyter notebook in the project is intend to build an image classifier using the VGG16 pre-trained model and compare its performance with the ResNet50 pre-trained model.


### 1 Design a classifier using the VGG16 pre-trained model

1 Import libraries, modules, and packages you will need. Make sure to import the preprocess_input function from keras.applications.vgg16.
2 Use a batch size of 100 images for both training and validation.
3 Construct an ImageDataGenerator for the training set and another one for the validation set. VGG16 was originally trained on 224 × 224 images, so make sure to address that when defining the ImageDataGenerator instances.
4 Create a sequential model using Keras. Add VGG16 model to it and dense layer.
5 Compile the mode using the adam optimizer and the categorical_crossentropy loss function.
6 Fit the model on the augmented data using the ImageDataGenerators.

### 2 Evaluate deep learning models on a test data

1 Load your saved model that was built using the ResNet50 model.
2 Construct an ImageDataGenerator for the test set. For this ImageDataGenerator instance, you only need to pass the directory of the test images, target size, and the shuffle parameter and set it to False.
3 Use the evaluate_generator method to evaluate your models on the test data, by passing the above ImageDataGenerator as an argument. 
4 Print the performance of the classifier using the VGG16 pre-trained model.
5 Print the performance of the classifier using the ResNet pre-trained model.

### 3 Prediction

Use the predict_generator method to predict the class of the images in the test data, by passing the test data ImageDataGenerator instance defined in the previous part as an argument. 
