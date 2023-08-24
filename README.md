# Water Bodies Segmentation in Satellite Images  |      Binary Image Segmentation

Kaggle Notebook: https://www.kaggle.com/code/shirshmall/water-body-image-segmentation-u-net-arch/notebook

#### **Description:**
This project centres around the precise delineation of water bodies within satellite images captured by the Sentinel-2 Satellite. Each image is accompanied by a monochromatic mask in which areas of water are depicted in white, while non-water regions are represented in black. The generation of these masks involved the computation of the Normalized Water Difference Index (NWDI), a metric conventionally utilized for identifying and quantifying vegetation in satellite images. However, a more stringent threshold was employed to effectively identify water bodies.

#### **Problem Statement:**
The primary objective of this project is to perform accurate segmentation of water bodies within the provided satellite images. The process entails the implementation of robust data preprocessing techniques, the development of a specialized neural network architecture, and the utilization of a suitable evaluation metric to gauge the quality of segmentation achieved.

#### **Approach:**

1. **Data Preprocessing:** Prior to model training, a series of data preprocessing steps were executed. This encompassed resizing, cropping, and reshaping the images to dimensions amenable for neural network input. Additionally, binary masking was applied to the water body masks to distinguish areas of interest from the background.

2. **Model Architecture:** The project adopted a U-Net architecture, meticulously constructed using the TensorFlow framework. The U-Net's distinctive design facilitates the creation of high-resolution segmentation maps, making it a fitting choice for this task. The architecture was built from scratch, enabling complete customization to suit the specific requirements of the project.

3. **Training and Evaluation:** The neural network was trained on the preprocessed dataset to learn the intricate spatial patterns indicative of water bodies. During training, the Intersection over Union (IOU) metric was employed to quantify the model's segmentation accuracy. IOU provides insight into the extent of overlap between predicted and ground truth masks, serving as an effective measure of segmentation performance.

#### **Results:**

Upon model convergence, the project achieved a commendable IOU score of 0.75. This metric signifies the substantial alignment between the predicted and actual water body segments. The results substantiate the effectiveness of the custom-built U-Net architecture in accurately segmenting water bodies from Sentinel-2 satellite images.

#### **Significance:**

Accurate segmentation of water bodies within satellite images holds significant importance across numerous applications, including environmental monitoring, urban planning, and disaster management. This project's success in achieving high-quality segmentation underscores its potential utility in real-world scenarios where the precise identification of water bodies is imperative.

By meticulously addressing data preprocessing, selecting an apt neural network architecture, and employing a suitable evaluation metric, this project contributes to the advancement of image segmentation techniques in the realm of remote sensing and geospatial analysis.

Dataset(contains images and masks) link: https://files.taskade.com/attachments/1b3ae25f-6ed9-4800-83f0-57043d9faf14/original/Segmentation%20Dataset.zip?_ga=2.232634015.1092276557.1671248657-2084344612.1657808593
