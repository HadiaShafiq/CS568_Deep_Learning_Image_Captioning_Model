# CS568_Deep_Learning_Image_Captioning_Model

We use two techniques mainly CNN and LSTM for image caption generation. We used the pre-trained model Inception. LSTM will use the information from CNN to help generate a description of the image.

### Dataset
Flicker8K dataset is used. Flickr8k data set is a public benchmark dataset for image to sentence description. This data set consists of 8000 images with five captions for each image.

###  Experimental Details
Batch Size: 30
Epochs: 10
Training Images: 6000
Testing Images: 1000

#### Feature Extraction Model
Inception V3 Model is used for extracting features of images. Resizing is done on images to make them of size (299,299,3). The features were stored on a file using pickle.

#### Caption Generation
For Generating Caption, We used LSTM model. 

### Evaluation
To evaluate our model, we tested some of the images to generate caption. The results were somewhat below average because of less training data and less epochs. When generating caption, some captions generated did not make sense.

