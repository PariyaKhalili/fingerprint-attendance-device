# fingerprint-attendance-device - Pariya Khalili

This project involves a computer vision task in a Jupyter Notebook. This project implements a Few-Shot Learning algorithm for a Time and Attendance device on the SOCOFing dataset from Kaggle (https://www.kaggle.com/datasets/ruizgara/socofing).

## 📁 Project Structure:

1. The SOCOFing dataset is loaded.
![Examples](https://github.com/PariyaKhalili/fingerprint-attendance-device/blob/main/images/image%201.jpg)

2. The user is assumed to enter 5 fingerprints for the device to identify them.
3. The 5 different attempts are 3 rotations with a random angle, a Gaussian noise, and a cropped center
4. These 5 functions are applied on the dataset for every fingerprint, and 350 IDs are created.
![Examples](https://github.com/PariyaKhalili/fingerprint-attendance-device/blob/main/images/image%202.jpg)

5. The positive and negative pairs are created.
6. The Siamese network with a ResNet50 as a feature extractor is created.
7. he network is trained with the trained data, and then retrained with the support set.
8. Then the network is tested with the query set.


