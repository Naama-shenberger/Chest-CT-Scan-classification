# Chest-CT-Scan-classification
It was a project about breast cancer detection using machine learning.
we classify and diagnose if the patient have cancer or not using AI model.
As part of the project, a quality CNN network was developed, that includes:

• Augmentation

• Several stages of training

• Monitoring of training.

• Optimization of hyper parameters.

• Execution of Classifier based on features from the network.
# DATA:
Data split:

train 70 % 

validation  10 %

test 20%




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



# ResNet-50 Model:

ResNet-50 is a convolutional neural network that is 50 layers deep. ResNet, short for Residual Networks.
The resnet 50 architecture contains the following element:

1. A convoultion with a kernel size of 7 * 7 and 64 different kernels all with a stride of size 2 giving us 1 layer.
2. Next we see max pooling with also a stride size of 2.
3. In the next convolution there is a 1 * 1,64 kernel following this a 3 * 3,64 kernel and at last a 1 * 1,256 kernel, These three layers are repeated in total 3 time so giving us 9 layers in this step.
4. Next we see kernel of 1 * 1,128 after that a kernel of 3 * 3,128 and at last a kernel of 1 * 1,512 this step was repeated 4 time so giving us 12 layers in this step.
5. After that there is a kernal of 1 * 1,256 and two more kernels with 3 * 3,256 and 1 * 1,1024 and this is repeated 6 time giving us a total of 18 layers.
6. And then again a 1 * 1,512 kernel with two more of 3 * 3,512 and 1 * 1,2048 and this was repeated 3 times giving us a total of 9 layers.
7. After that we do a average pool and end it with a fully connected layer containing 1000 nodes and at the end a softmax function so this gives us 1 layer.

We don't actually count the activation functions and the max/ average pooling layers.

so totaling this it gives us a 1 + 9 + 12 + 18 + 9 + 1 = 50 layers Deep Convolutional network.
# results:
The results is reported as the accuracy of each classifier, using the following metrics when these are applicable:

• precision

• recall

• F1-score

• Accuracy

• Plot

# Explanation of project files:
1.  Chest CT-Scan images Dataset:
The model for the 4 Categories
2. Chest CT-Scan images Dataset 2:
The model for 2 Categories
3. Chest CT-Scan images Dataset 3:
The model for 3 Categories
4. Data:
The data for 4 Categories
5. Data 2:
The data for 2 Categories
6. Data 3:
The data for 3 Categories
7. Data_jpg:
Folder images for visualization in jpg format
8. ResNet50_2.Categories.ipynbg:
Model for the 4 categories- Adenocarcinoma, normal cell
9. ResNet50_3.Categories.ipynb:
Model for the 3 categories- Adenocarcinoma, Large cell carcinoma, Squamous cell carcinoma
10. ResNet50_4.Categories.ipynb:
Model for the 4 categories- Adenocarcinoma, Large cell carcinoma, Squamous cell carcinoma, normal cell
