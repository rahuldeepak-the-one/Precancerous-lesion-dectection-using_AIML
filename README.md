
# Precancerous Lesion Detection using AI/ML
The Aim of the project is to Implement the semi-supervised Algorithm Mixmatch to label differnent images of skin cancer into 7 major types namely (akiec, bcc, bkl, df, mel, nv, vasc)

## Datasets Used 
* Use this [link][https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T] to download the "The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions Version 4.0" 

* Download the first two datasets HAM10000_part_1 and HAM10000_part_2, Our main training and testing goes to this 10000 unlabelled images.

* Unzip and combine both folders and rename it as Image_set to use in the code 

* Download HAM10000_metadata.tab which is uesd as labels.csv, this .csv file contains all the labels for the 

* Test_images folder is used to test the images
## segregate_data.py
* This python file is used to divide the total 10000 images into X labelled and 10000-X unlabelled images

* We used a fraction of 20% images as labelled data and keep them in Images_set folder which contains 7 subfolders saperated by their respective 7 labels.

* Remaining unlabelled images are stored in unlabelled_images folder which are used for training and testing

## supervised_resnet.ipynb

* The code in this file consisits of 4 parts
  - part_1 : Splitting of Datasets
  - part_1 : Training and testing of Supervised Model
  - part-2 : Implementation of Mixmatch 
  - part-3 : Training and testing of Mixmatch

Run the code on order, the training and testing accuracies for both are printed under the Headings 
