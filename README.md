# Automatic detection of Colon polyps 
The human gastrointestinal (GI) tract is made up of different sections, one of them being the large bowel. Several types of anomalies and diseases can affect the large bowel, such as colorectal cancer. Colorectal cancer is the second most common cancer type among women and third most common among men. Polyps are precursors to colorectal cancer, and is found in nearly half of the individuals at age 50 having a screening colonoscopy, and are increasing with age. Colonoscopy is the gold standard for detection and assessment of these polyps with subsequent biopsy and removal of the polyps. Early disease detection has a huge impact on survival from colorectal cancer, and polyp detection is therefore important. In addition, several studies have shown that polyps are often overlooked during colonoscopies, with polyp miss rates of 14%-30% depending on the type and size of the polyps. Increasing the detection of polyps has been shown to decrease risk of colorectal cancer. Thus, automatic detection of more polyps at an early stage can play a crucial role in improving both prevention of and survival from colorectal cancer.
Polyps are lesions within the bowel detectable as mucosal outgrows. The polyps are either flat, elevated or pedunculated, and can be distinguished from normal mucosa by color and surface pattern. Most bowel polyps are harmless, but some have the potential to grow into cancer. Detection and removal of polyps are therefore important to prevent development of colorectal cancer. Since polyps may be overlooked by the doctors, automatic detection would most likely improve examination quality. Automatic computer aided detection of polyps would be valuable both for diagnosis, assessment and reporting.
Since the number of images included in the dataset is small, up to 1000 images only, a methodology was used to generate more images using Gaussian blur more than once and each time it was used for a greater and greater degree of blur.
The goal of using a Gaussian blur is to make the neural network also focus on the outline and try to locate the polyps despite the blur in the image.
On the other hand, an improved neural structure was used for the U-NET model, so that the proposed structure helped to locate the polyps with higher accuracy.
As we know, we are studying the ability to locate polyps that can develop into malignant cancer.
# Dataset Used:
## Dataset Link: 
https://datasets.simula.no/kvasir-seg/
## Samples of Dataset:
| An example of polyps | Dataset samples |
| :---: | :---: |
| ![colon-AdobeStock_48336100-1-1024x768](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/16c7a10f-c803-48dd-8b19-4cdd867cda30)|![download (1)](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/6b980242-a035-42bd-ad28-eaabf7665dcd)|

# Neural network architecture proposal:
![architecture segmentation drawio (4)](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/fa41b5fc-ee45-448c-9d89-4d0e779156a4)

# Results and metrics:
| # | Metrics |
| :---:   | :---: |
| Evaluation on Training and Validation Data |  ![image](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/480ce004-e7ee-4db2-a642-6ed9ef1060b7) ![image](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/909044aa-6579-4964-b05a-d65dd5267f43)|
| Classification Report, Accuracy Score, Precision Score, Recall Score, dice Score |  ![image](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/e770b3ae-c493-4945-9886-ef7b02baaa9d) ![image](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/cb1473f6-8109-40b9-871f-d6822cb63b32)|

## Visual review of the results:
| # Samples of Validation Data (compare the predicted masks with the true masks)    |
| :---: |
| ![download (2)](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/34089eb8-bf94-413d-84b9-27afd6338630)|
|![download (3)](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/08b9ef44-92a9-4e5e-b3dc-2035f88241f5)|
|![download (4)](https://github.com/kaledhoshme123/Automatic-detection-of-Colon-polyps-/assets/108609519/d2f2b955-d046-458b-b489-4f259f51fc97)|



