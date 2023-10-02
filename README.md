# Chest X-Ray Analysis using Deep Learning

***Name :*** Shayaan Hussain <br/>
***Hall Ticket Number :*** 19K41A04E6 <br/>
***Year/Sem :*** 4/2 <br/>
***Major Project :*** B.Tech ECE-C Team 6 (2023 Batch)<br/>
***Project Title :*** ENHANCED DETECTION OF PULMONARY AILMENTS USING MACHINE LEARNING ALGORITHMS<br/>
***College :*** S R Engineering College<br/><br/>
***IEEE Publication :*** <a href="https://ieeexplore.ieee.org/document/10169625">Click Here</a>

This project was submitted as Major Project for award of the degree Bachelor of Technology in Electronics and Communication Engineering (ECE) in the academic year 2022-2023.<br/><br/>

## ***About the Project:***
Two deep learning models, namely VGG-19 and a Custom CNN were developed in order to classify a chest x-ray image as Normal, Pneumonia infected or Tuberculosis infected.<br/><br/>

## ***About the Dataset Used:***
Two datasets were used from kaggle.<br/><br/>
Dataset 1 : www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia<br/>
This dataset consists of 5,856 images, 4273 images diagnosed as Pneumonia and 1583 images diagnosed as no disease.<br/><br/>
Dataset 2 : www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset<br/>
This dataset consists of 4200 images, 700 images diagnosed as Tuberculosis and 3500 images diagnosed as no disease.<br/><br/>
Out of these 10056 images collected from above datasets, a total of 1830 images were selected at random to train, validate and test the model. 500 images of each class were used for training, 10 were used for validation and 100 were used for testing. These 1830 images can be found in Images directory<br/><br/>

## ***Results Acheived:***
#### ***<b>VGG-19 Model:<b/>***
Accuracy achieved on Training Data : 97.0%<br/>
Accuracy achieved on Validation Data : 96.6%<br/>
Accuracy achieved on Testing Data : 96.6%<br/><br/>

#### ***<b>Custom CNN Model:<b/>***
Accuracy achieved on Training Data : 93.6%<br/>
Accuracy achieved on Validation Data : 100%<br/>
Accuracy achieved on Testing Data : 89%<br/>

## ***To run this code:***
The code was executed on jupyter notebook with ***<b>python 3.9.10<b/>***<br/>
To install all the dependancies, run the following shell command :<br/>
```
pip install -r requirements.txt
```
To run the code to train the Custom CNN model, execute all the cells in ```code1_customModel.ipynb``` file. <br/>
To run the code to train the VGG-19 model, execute all the cells in ```code2_vggModel.ipynb``` file. <br/>

### ***Note:***
1. There are two cells of evaluation in both files i.e. ```code1_customModel.ipynb``` and ```code2_vggModel.ipynb```, the first one represents the fully trained model i.e. the model after running all the epochs and the second one represents the best model saved throughout the training process based on the validation loss.
2. VGG-19 Model files were larger than 100MB which is the limit for uploading files on github, hence they were removed from this repository. Kindly use the weights file to make predictions as specified in 9th cell of the file ```code3_predictions.ipynb``` [VGG-19 Model Prediction (Method 2)]<br/>
