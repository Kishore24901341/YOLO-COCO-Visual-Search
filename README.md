# YOLO Image Search System

## ABSTRACT 
The YOLO Image Search System is an AI-powered computer vision application designed to perform object detection, metadata generation, and image retrieval using YOLOv11. The system processes image datasets, detects objects present in images, stores detection information as structured metadata, and enables users to perform intelligent searches using object-based filters.
The application provides an interactive Streamlit UI, allowing users to:

Process new image datasets

Run object detection using YOLOv11

Generate searchable metadata

Apply logical filters (AND / OR)

Retrieve matching images instantly

Export results as JSON

The project aims to improve image organization and searchability using modern object detection techniques.
## Dataset & YOLO Model Details (COCO)
This project uses the COCO (Common Objects in Context) dataset classes supported by YOLOv11.

COCO contains 80 object categories, including:
```
Person
Car
Dog
Cat
Airplane
Banana
Bicycle
Chair
Bottle
Laptop
YOLO Model Used
```
### Model: YOLOv11

### YOLOv11 is a state-of-the-art object detection model optimized for:
```
High detection accuracy
Real-time inference
Faster processing
Improved scalability
```
### The model performs:
```
Object Detection
Bounding Box Prediction
Class Identification
Confidence Score Generation
Detection outputs are converted into metadata for image querying.
```

## Environment Setup
Before running the project, install:

### Prerequisites
Python 3.11

Anaconda / Miniconda

Visual Studio Code (VS Code)

NVIDIA GPU (Optional – for GPU acceleration)

### Open the project folder inside VS Code.

#### Required project files:
```
requirements.txt
instructions.txt
app.py
```
### Open terminal in VS Code:
```
View → Terminal
```

## GPU Installation Steps

### Step 1 – Create Conda Environment
```
conda create -n yolo-image-search-gpu python=3.11 -y
```
### Step 2 – Activate Environment
```
conda activate yolo-image-search-gpu
```
### Step 3 – Install PyTorch with CUDA Support
```
conda install pytorch torchvision pytorch-cuda=12.4 -c pytorch -c nvidia
```
### Step 4 – Install Project Dependencies
```
pip install -r requirements.txt
```
## How to Run in VS Code using Conda
### Activate Environment
```
conda activate yolo-image-search-gpu
```
### Launch the Streamlit interface
```
streamlit run app.py
```
### The terminal will display and Open Browser:
```
Local URL: http://localhost:8501
```
### Features Available in UI
Upload image dataset

Select YOLOv11 model

Process images

Generate metadata

Apply search filters

Display results grid

Export JSON output

## Output
### UI Screenshot
<img width="1901" height="900" alt="image" src="https://github.com/user-attachments/assets/c4f57d76-3979-4eee-9c10-a34fc93790a3" />

### Object Detection Output
<img width="1920" height="1020" alt="Screenshot 2026-05-25 160756" src="https://github.com/user-attachments/assets/3c065d2e-25a3-426d-b8b4-e13fc8d91e7f" />

<img width="1920" height="1020" alt="Screenshot 2026-05-25 160802" src="https://github.com/user-attachments/assets/1d6821b2-8fe2-4948-baa2-08d7534113bf" />

<img width="1920" height="1020" alt="Screenshot 2026-05-25 160813" src="https://github.com/user-attachments/assets/3167e7fe-2333-44b0-a3a5-36fea7890409" />

### VS Code Terminal Output
<img width="1919" height="1022" alt="Screenshot 2026-05-26 103131" src="https://github.com/user-attachments/assets/78747f74-d24d-485d-9300-7467c83da542" />

<img width="1919" height="1017" alt="Screenshot 2026-05-26 103146" src="https://github.com/user-attachments/assets/176a74fa-7299-4970-a57b-b28ecc294d31" />

## Enhancements
The system goes beyond basic object detection by introducing metadata-based image searching. Detection outputs are stored in JSON format, allowing fast querying without rerunning inference. The application also supports logical filtering using AND/OR conditions, threshold-based searches, and loading previously generated metadata for quicker execution. The modular pipeline improves scalability and maintainability.

## Conclusion
The project demonstrates how YOLOv11 object detection, metadata engineering, and interactive deployment can be combined to build an efficient image search application.

The modular pipeline architecture improves:

Scalability

Maintainability

Usability

Performance

### Future improvements may include:

Semantic search

Multi-model support

Cloud deployment

Database integration

Real-time video search
