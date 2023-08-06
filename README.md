# Determine the location of the skin lesion spread
- Dermatologists suffer from the difficulty of locating cancerous and malignant skin lesions, which causes many problems during the process of removing the tumor, which leads to the return of the tumor again. In determining the location of the tumor and its spread and determining the area that must be removed accurately.
- The proposed neural architecture, which is based on convolutional neural networks, extracts the basic features of the skin lesion and then generates and defines the lesion area based on the extracted features from the lesion area.
- The proposed model was able to reach a high accuracy in determining the location of the spread of the cancerous tumor, or the location of the spread of the skin lesion.
- The dataset used in the study includes 10,000 images and masks for 7 types of skin lesions, as follows:

1. *Actinic keratoses and intraepithelial carcinoma / Bowen's disease (AKIEC).*
2. *basal cell carcinoma (BCC).*
3. *benign keratosis-like lesions (solar lentigines / seborrheic keratoses and lichen-planus like keratoses, BKL).*
4. *dermatofibroma (DF).*
5. *melanoma (MEL).*
6. *melanocytic nevi (NV).*
7. *vascular lesions (angiomas, angiokeratomas, pyogenic granulomas and hemorrhage, VASC).*

- Data Augmentation was used to generate more images by rotating the images horizontally and vertically, and thus 30,000 images and 30,000 masks were obtained, 3,500 of which were used for verification during training the neural network and adjusting its parameters, and 1,000 were used to test the neural network after training.
- An important addition to the neural network has been used, which is to predict the type of skin lesion at the same time that the mask is generated for the area of ​​the spread of the skin lesion, because the imposition of an addition task on the neural network is linked to the basic task and helps the neural network to access the basic features that are included in the images It facilitates the generation of the mask (which determines the location of the skin lesion).
# Dataset Used:
## Dataset Link: 
https://www.kaggle.com/datasets/surajghuwalewala/ham1000-segmentation-and-classification
## Samples of Dataset:
| Dataset Samples with Data augmentation |
| :---: |
| ![download (9)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/3fa3cd9e-4d62-43f6-958e-4df9195abb83)|

# Neural network architecture proposal:
![architecture segmentation drawio (6)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/2ebc3c1a-6f3d-4b40-89c0-4ff7fce9d4a4)

# Results and metrics:
| # | Metrics |
| :---:   | :---: |
| Evaluation on Test and Validation Data |  ![image](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/935098e4-f898-443f-a066-133c0622ed5c) ![image](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/ff11beb2-8e0f-4a33-be76-c6c2bcb23b69)|
| Classification Report, Accuracy Score, Precision Score, Recall Score, dice Score on Test Data|  ![image](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/240939eb-292d-4060-8c61-4c30b396160e) ![image](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/6cfd9ce5-b1b5-4bbc-a14e-1320627d9758)|
| Classification Report, Accuracy Score, Precision Score, Recall Score, dice Score on Validation Data|  ![image](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/16406928-b226-4216-80c0-11c025394e23) ![image](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/40c621d4-9072-4a97-b9d0-cbbf6d992206)|

## Visual review of the results:
| # Samples of Validation Data (compare the predicted masks with the true masks)    |
| :---: |
| ![download (10)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/caa7574e-4910-4856-a174-923e2c12f738)|
| ![download (11)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/8e201f25-8fd9-478c-9ee9-67f4342afe05)|
| ![download (12)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/39b900c4-e454-40c5-a3f4-d830ea38077b)|
| ![download (13)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/07865f29-5cbc-48ed-90c2-f1e1cec68bca)|
| ![download (14)](https://github.com/kaledhoshme123/Determine-the-location-of-the-skin-lesion-spread/assets/108609519/dd327c4a-8ba2-46d6-a657-c5c1d167e9f2)|




