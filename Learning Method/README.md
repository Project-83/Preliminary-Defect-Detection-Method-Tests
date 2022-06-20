
This method of defect detection is a modified version which was initially developed by [Emre Okcular and Hashneet Kaur](https://github.com/emreokcular/textile-defect-detection)

# Models
Three models were created which are: 
 - Simple CNN
 - ResNet 18
 - Resnet 34

# Dataset

The dataset that was used for training and testing are found on [Kaggle](https://www.kaggle.com/datasets/belkhirnacim/textiledefectdetection).
The dataset is 4 GB and has 48000 images. The size of the images in the dataset is either 32x32 or 64x64. The data includes records that belong to 6 different classes of defects:
 - Good - If the fabric is good and has no defect
 - Colour - There is a defect in the colour of the fabric
 - Cut - There is a cut in the fabric
 - Hole - There is a hole in the fabric
 - Thread - There is some thread coming off
 - Metal Contamination - Fabric has some metal contamination
 
Each of the images are also rotated to 8 different agnles:
  - 0°
  - 20°
  - 40°
  - 60°
  - 80°
  - 100°
  - 120°
  - 140°

## Sample Images from Dataset

Images from each defect class are shown below.

| Good | Colour | Cut | Hole | Thread | Metal Contamination |
|------|--------|-----|------|--------|---------------------|
|  ![image](https://user-images.githubusercontent.com/67822005/174516555-e2b49b30-40bf-429a-bc72-a3739e2e88e0.png)     |   ![image](https://user-images.githubusercontent.com/67822005/174516674-14a2ecc0-71f5-4a39-ac72-223ea1917fbd.png)     |   ![image](https://user-images.githubusercontent.com/67822005/174516736-3b252909-c63e-4f33-b6da-1808f96a8df3.png)  |  ![image](https://user-images.githubusercontent.com/67822005/174516992-970afb43-fcad-4d1f-89d8-209a68129bc3.png)    |   ![image](https://user-images.githubusercontent.com/67822005/174517140-e27a785f-818c-4cfc-b4d5-afb705224da3.png)     |           ![image](https://user-images.githubusercontent.com/67822005/174516912-12b09744-0364-488e-ab73-e0db27967724.png)          |


# Results

The results for each of the different models are summarised in the tables below

## Simple CNN
| **Defect Class** | Good | Colour | Cut | Hole | Thread | Metal Contamination |
|------------------|------|--------|-----|------|--------|---------------------|
| **Accuracy(%)**  |64.75 |80.06   |64.06|23.56 |46.8    |97.06                |


## ResNet18
| **Defect Class** | Good | Colour | Cut | Hole | Thread | Metal Contamination |
|------------------|------|--------|-----|------|--------|---------------------|
| **Accuracy(%)**  |94.38 |93.69   |55.56|34.69 |47.94   |93.25                |

## ResNet34
| **Defect Class** | Good | Colour | Cut | Hole | Thread | Metal Contamination |
|------------------|------|--------|-----|------|--------|---------------------|
| **Accuracy(%)**  |90.06 |89.88   |65.06|42.44 |39.44   |89.25                |





