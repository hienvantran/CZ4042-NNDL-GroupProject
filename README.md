# CZ4042-Gender Classification

## Project overview

Automatic gender classification has become prevalent in many digital applications, whether in monitoring systems or on social platforms for image analysis. This demands the increase in performance accuracy of gender classification.
With the rise in computational power and availability of large datasets of labeled images, neural networks have been used to extract human attributes from images, such as gender and age. Recent advancements in image classification with the use of convolutional neural networks and new architectures may be useful in improving gender classification, and will be the focus in this project.

The goal of this project is two-fold:

1. Explore neural network architectures to improve the accuracy of gender classification
2. Consider age and gender recognition simultaneously to take advantage of the gender-specific age
   characteristics and age-specific gender characteristics inherent to images

The dataset used to benchmark models against is the Adience dataset.

## Technical Details

In this project, we implement several methods to classify gender from images:

1. Gender detection with pre-trained models: Inceptionv3, ResNet, VisTrans
2. Gender detection by transfer learning from CelebA dataset with pre-trained models: Inceptionv3, ResNet, VisTrans
3. Age-gender multi-task learning.
4. Data augmentation: rand and mixup

For method details and results, please refer to CZ4042 Report.pdf.

## File Structure

1. CZ4042 Report.pdf : Group Project report
2. cz4042-project-eda.ipynb : Notebook to run Exploratory Data Analysis
3. cz4042-project-rand_mixup_augmentation.ipynb: Notebook to run Data Augmentation techniques
4. cz4042-age-gender-hyperparam.ipynb: Notebook to run age-gender multi-task learning and age-gender hyperband experiments for Inceptionv3.
5. cz4942-gender-transfer-learning.ipynb: Notebook to run directly train on Adience and Transfer Learning from CelebA to Adience for Resnet, Inceptionv3, Inception-Resnetv2, Vision Transformer.

The data used in the notebook is listed here:

1. Adience Benchmark Gender And Age Classification: https://www.kaggle.com/datasets/ttungl/adience-benchmark-gender-and-age-classification
2. CelebFaces Attributes (CelebA) Dataset: https://www.kaggle.com/datasets/jessicali9530/celeba-dataset
3. CZ4042 Adience: https://www.kaggle.com/datasets/oongjiexiang/cz4042-adience
4. CZ4042 Task 2: https://www.kaggle.com/datasets/oongjiexiang/cz4042-task-2
5. CZ4042-transfer-learning : https://www.kaggle.com/datasets/lyantran/cz4042transferlearning
6. CZ4042-age-gender: https://www.kaggle.com/datasets/lyantran/cz4042agegender

The 1,2,3 dataset links are all the datasets we used for our model training process.
The 4 dataset contains the weight for direct training on Adience dataset for Resnet, Inceptionv3, Inception-Resnetv2, Vision Transformer.
The 5 dataset contains the weight for transfer learning from CelebA on Adience for Resnet, Inceptionv3, Inception-Resnetv2, Vision Transformer.
The 6 dataset contains the weight for age-gender multi-task learning and age-gender hyperband experiments for Inceptionv3.

If you cannot see the datasets links, please email HIENVAN001@e.ntu.edu.sg.
