# PlantVillage Leaf Disease Classification (CNN / Transfer Learning)

## Overview
This project builds an image classification model to detect plant leaf diseases using the **PlantVillage** dataset.  
The dataset is split into training/validation/test folders using `splitfolders`, and a CNN / transfer learning pipeline is trained and evaluated using TensorFlow/Keras.

## Dataset
**Dataset name:** PlantVillage (image dataset)

### Expected folder structure
The notebook expects this structure after splitting:

data_split/
train/
class_1/
class_2/
...
val/
class_1/
class_2/
...
test/
class_1/
class_2/
...


### How the split is created
The notebook uses:
- Input folder: `PlantVillage/`
- Output folder: `data_split/`
- Split ratio: **70% train, 10% validation, 20% test**

## Steps Performed
1. Split dataset into train/val/test using `splitfolders`
2. Load images using `ImageDataGenerator.flow_from_directory()`
3. Train CNN / Transfer Learning model (e.g., VGG16)
4. Evaluate performance on test set
5. Save best model as `best_model.h5` (if enabled)
6. Visualize class distribution and results

## How to Run
1. Download the PlantVillage dataset and place it in a folder named `PlantVillage/`
2. Open and run the notebook:
   `plantvillage_disease_classification.ipynb`
3. The notebook will create `data_split/` automatically and start training/evaluation.

## Model Output
- The notebook loads a saved model using:
  `best_model.h5`
- If `best_model.h5` is not included in the repo, you can generate it by training the model in the notebook.

## Technologies Used
- Python
- TensorFlow / Keras
- ImageDataGenerator
- splitfolders
- NumPy / Pandas
- Matplotlib

## Author
Abdul Bari Mohammed
