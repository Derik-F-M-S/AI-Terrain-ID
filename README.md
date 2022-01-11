# AI-Terrain-ID
## This was a competition project for the ECE542- Neural Networks course at NCSU. A CNN-LSTM-FCN model was developed to ID terrain being walked on from sensor data. This implementation scored 1st place in the class competition. 

## Description
This project was completed as part of a class competition for a course on Neural Networks where teams were tasked with creating a machine learning model to classify the type of walking activity that was being performed from walking on level ground, walking on grass, walking up stairs, and walking down stairs. The labeled trainning data was provided as a modified dataset from that found at https://ieee-dataport.org/open-access/lower-limb-prostheses-environmental-context-dataset. Separate unlabeled testing data was provided and groups were tasked with obtaining the best F1 score on this data through the use of any Neural Network models they saw fit. 

## Implementation

This implementation uses a CNN-LSTM model to extract features from the raw IMU data and clssify it as labels 0,1,2,3 representing the type of terrain being walked on. 
The data is also preprocessed using the robustscaler from the sklearn.preprocessing python module and RandomUnderSampler class from the imblearn Python module. The predictions are also filtered using a mode filter for cleaner outputs. 

## Dependencies

