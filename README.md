# ChickCheck Machine Learning Documentation
ChcikCheck applies the machine learning model as technology in image classification to determine the type of disease that infects chickens. Classification of disease types was carried out based on images of chicken droppings.
#### This is the step to build the model
- Collect a data set of chicken droppings
- Split the data set into 90% for the training set and 10% for the validation set
- Create a machine learning model with CNN (Convolutional Neural Network) using the Xception architecture as the base model
- Train the model
- Evaluation of machine learning models
- Test the model with new test data that the model has never seen before
- Convert model in TensorFlow.Js
- Deploy models using API

## Dataset
The dataset used in this project is a collection of images of chicken droppings. The number of datasets used is 2.361 which is divided into 4 classes
1. Coccidiosis
2. New Castle Disease
3. Salmonella
4. Healthy

## Libraries
1. **TensorFlow**: Open source machine learning framework for creating and refining machine learning models.
2. **Keras**: High-level interface for model development and training that is constructed on top of TensorFlow.
3. **NumPy**: Fundamental library that is used for efficient array manipulation and math operations.
4. **Matplotlib**: A complete Python visualization toolkit.

## Model Architecture
This project employs transfer learning with the Xception architecture:
- **Base Model**: Utilizes a pre-trained Xception model with ImageNet weights, excluding the top layers
- **Freezing Layers**: Some layers are frozen to retain pre-learned features and prevent retraining.
- **Customization**: Additional layers (Global Average Pooling, Dense, Dropout) are added for task-specific adaptation.

![image](https://github.com/ChickCheckTeam/chickcheck-machine-learning/assets/94920692/37096194-12d2-4da3-8e4e-7b4d27cdd142)

## Model Peformance
Model training results are measured using matrix accuracy

**Training Accuracy**: Achieved 98.08% accuracy on the training data set.

**Validation Accuracy**: balances the training process with 93.70% accuracy on validation data.

![image](https://github.com/ChickCheckTeam/chickcheck-machine-learning/assets/94920692/12b237f6-5771-4963-8ee6-8f80d534e836)

## Model Evaluation and Testing 
Model testing is carried out using test data. Classification results based on class are shown in the confusion matrix.

![image](https://github.com/ChickCheckTeam/chickcheck-machine-learning/assets/94920692/f7542a96-1d7f-48f1-bec1-0e2cdfeae1d3)

