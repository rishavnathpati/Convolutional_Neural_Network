# Convolution_Neural_Network
This is an implementation of the CNN, for handwritten character recognition (a-z, A-Z, 0-9), after referring from various online tutorials and codes. This is just a test implementation to understand the working of the CNN. It has been implemented using Tensorflow and is not structured to be used directly. You can refer to this model and device it in your own way.<br/>
I have averaged its performance over the test set in the form of batches, and it has a 92.8% accuracy (quite low). Though it has been trained only 12 epochs. You can train it more no. of times from the main program.<br/>
The new_train_CNN.py is the main program to start from. It has options where it asks yoou to 1. train, 2. test, 3. predict.<br/>
It is based on the Extended-MNIST dataset, which is available for download from Kaggle. You can head over to Kaggle for more options regarding the choice of dataset related to handwritten character recognition. I had the emnist-letter-train.csv and emnist-letter-test.csv where the no. of classes were 37.<br/>
Note: This is not some structured implementation of CNN for easy reuse. This is just to get the idea of the working of the CNN.<br/>
File description:<br/>
ConvolutionNetwork.py --> Include the code definig each component of the convolution block. The code for the structure of the Conv Layer, Pooling Layer, Activation Layer, Dense Layer and the Softmax function is defined here.<br/>
Simple_CNN.py --> It is a simple CNN with three Convolution Block: [5X5 32 filters] -> [5X5 64 filters] -> [5X5 128 filters] -> [200 nodes Dense Layer] -> [200 nodes Dense Layer] -> Softmax Layer.<br/>
new_train_CNN.py --> Contains the code for training, testing of the network and predicting of character. It is more-or-less commented to help you understand the working sequence.<br/>
Dataset_Generator.py --> Helps to read the data from .csv files. I have the code to read the dataset fromt the .csv file and store it in as array, so that during re-traininng or re-testing, I don't have to read from the .csv file again and store in an array. Thus the files: train_data_file.py, train_lable_file.py and test_data_file.py, test_label_file.py will be created only once.<br/>
image_preprocess_wCV2.py --> This include all the preprocessing needed to be done to the image to be predicted, using the CV2 library.<br/>
Thats probably all of it.<br/>
There are some other simple implementation of the CNN that might be easier to understand. But this implementation is more regarding understanding the steps of working of the CNN. If there is any problem, you can mail me your question.<br/>
