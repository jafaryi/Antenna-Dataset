# Antenna-Dataset
This dataset is prepared for YOLO object detection model training, specifically focused on detecting antennas. 

The dataset contains two subsets:
1. General Antenna Dataset (`antenna_dataset`): Includes training and validation data with images and YOLO-format labels.
2. Data with Sunlight Effects (`Data with sunlight`): Includes training and testing data under challenging lighting conditions (e.g., direct sunlight), separated into images and labels.

All annotations in this dataset were auto-annotated and have not been manually reviewed or corrected.

Annotations are provided in YOLO format to ensure compatibility with YOLO training pipelines.




Data Source :
The images in this dataset were collected from publicly available YouTube videos. These videos were carefully selected to ensure a diverse and representative collection of antenna-related images.

Dataset Link :
You can download the dataset from the following link: [Dataset Link]( https://drive.google.com/file/d/1jFjSSOv4nJ_-z-rTVW3mcS-uE5K7S9_p/view?usp=sharing)


## Dataset Structure
The dataset is organized as follows:

1. **General Antenna Dataset (`antenna_dataset`)**
   - This folder contains the general dataset images and annotations used for training and validating YOLO models in typical conditions.
   - Subdirectories:
     - **`train/`**: Contains the training data.
       - `images/`: The training images.
       - `labels/`: YOLO-format annotations corresponding to the training images.
     - **`valid/`**: Contains the validation data.
       - `images/`: The validation images.
       - `labels/`: YOLO-format annotations corresponding to the validation images.

2. **Data with Sunlight Effects (`Data with sunlight`)**
   - This folder focuses on antenna data under challenging lighting conditions (e.g., direct sunlight) to improve YOLO model robustness in such environments.
   - Subdirectories:
     - **`train/`**: Contains training data for antennas under sunlight.
       - `image/`: The training images with sunlight effects.
       - `label/`: YOLO-format annotations corresponding to the training images.
     - **`test/`**: Contains testing data for antennas under sunlight.
       - `image/`: The testing images with sunlight effects.
       - `label/`: YOLO-format annotations corresponding to the testing images.
      
![Dataset](https://github.com/user-attachments/assets/fde77bf1-6aff-4a08-b601-8ca69c3fb362)  
*Figure 1: Dataset*

## Installation
To download this dataset for YOLO training, follow these steps:

1. Clone this repository:
   ```bash
   git clone https://github.com/jafaryi/Antenna-Dataset.git


## BBox Tester

The repository includes a folder named `BBox_tester.rar` that contains Python scripts for testing bounding boxes and related functionalities. These scripts can be used to visualize and validate the bounding box annotations from the dataset.

### Scripts in the BBox Tester Folder

1. **`mytest.py`**  
   This script performs basic tests to visualize the bounding boxes over the images.  
   - **`path_pic`**: Specify the path to the folder containing your images (e.g., `./antenna_dataset/train/images`).
   - **`path_annotation`**: Specify the path to the folder containing YOLO-format annotation files (e.g., `./antenna_dataset/train/labels`).

2. **`test_BBox.py`**  
   This script visualizes bounding boxes using the dataset images and their corresponding annotations.

3. **`test.py`**  
   This script provides additional validation for YOLO annotations.

4. **`use_for_T3.py`**  
   This script is designed for specialized transformations or bounding box-related debugging tasks.




