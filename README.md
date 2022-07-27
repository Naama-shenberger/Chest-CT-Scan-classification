
# Chest CT classification

In this project we classify chest CT images, as part of the project we built a deep neural network (CNN).

## Features

- Augmentation
- Callbacks
- EarlyStopping 
- Hyperparameter optimization


## Data
We took the data from kaggle.

Link: https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

The data contain 3 chest cancer types 
1. Adenocarcinoma
Adenocarcinoma of the lung: Lung adenocarcinoma is the most common form of lung cancer
Adenocarcinomas are found in several common cancers, including breast, prostate and colorectal.
Adenocarcinomas of the lung are found in the outer region of the lung
in glands that secrete mucus and help us breathe.
Symptoms include coughing, hoarseness, weight loss and weakness.

2. Large cell carcinoma
Large-cell undifferentiated carcinoma: Large-cell undifferentiated carcinoma lung cancer grows and spreads quickly and can
be found anywhere in the lung. This type of lung cancer usually accounts for 10
to 15 percent of all cases of NSCLC.
Large-cell undifferentiated carcinoma tends to grow and spread quickly.

3. Squamous cell carcinoma
Squamous cell: This type of lung cancer is found centrally in the lung,
where the larger bronchi join the trachea to the lung,
or in one of the main airway branches.
Squamous cell lung cancer is responsible for about 30 percent of all non-small
cell lung cancers, and is generally linked to smoking.

4. And the last folder is the normal CT-Scan images
## Data Split
The data training set contains 70% of the data
 - adenocarcinoma size 195
 - large size 115
 - squamous size 155
 - normal size 148
Total: 613 images belonging to 4 classes

The data testing set contains 20% of the data
 - adenocarcinoma size 120
 - large size  51
 - squamous size 90
 - normal size 54
Total: 315 images belonging to 4 classes

The data validation set contains 10% of the data
 - adenocarcinoma size 23 
 - large size 21
 - squamous size 15
 - normal size 13
Total: 72 images belonging to 4 classes

## Transfer learning (TL)
  We used the ResNet-50 network which has 50 layers, the network is trained on more than a million images and can classify images into 1000 categories.

## Folder Structure
1.  Chest CT-Scan images Dataset:
The Data for the 4 Categories

2. Chest CT-Scan images Dataset 2:
The Data for 2 Categories

3. Chest CT-Scan images Dataset 3:
The Data for 3 Categories

4. Data_jpg:
Folder images for visualization in jpg format

5. ResNet50_2.Categories.ipynbg:
Model for the 2 categories- Adenocarcinoma, normal cell

6. Hyperparameters_3.Categories.ipynb:
Model for the 3 categories- Adenocarcinoma, Large cell carcinoma, Squamous cell carcinoma

7. ResNet50_4.Categories.ipynb:
Model for the 4 categories- Adenocarcinoma, Large cell carcinoma, Squamous cell carcinoma, normal cell
