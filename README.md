# Brain Tumor Detection UI

A machine learning application that uses a trained PyTorch model to classify brain MRI images. The application provides a simple Streamlit interface where users can upload an MRI image and receive a predicted tumor classification with a confidence score.

## About the Project

The Brain Tumor Detection UI was created to demonstrate how machine learning can be combined with a user-friendly web interface.

The application analyzes uploaded brain MRI images and classifies them into one of four categories:

- Glioma
- Meningioma
- Pituitary Tumor
- No Tumor

The project uses PyTorch for the machine learning model and Streamlit for the web interface.

## Features

- Upload brain MRI images
- Classify MRI images into four categories
- Display the predicted classification
- Display the model's confidence score
- Show prediction confidence with a visual bar chart
- Provide a doctor review message when confidence is low
- Simple Streamlit web interface

## Technologies Used

- Python
- PyTorch
- Streamlit
- NumPy
- Pillow (PIL)
- Matplotlib
- Machine Learning / Deep Learning

## How It Works

1. The user uploads a brain MRI image.
2. The application prepares the image for the machine learning model.
3. The trained PyTorch model analyzes the image.
4. The model predicts one of four classifications.
5. The application displays the prediction and confidence score.
6. If the confidence is low, the application recommends professional review.

## Project Structure

```text
BrainTumorUI/
│
├── app.py
├── pipeline.py
├── utils.py
├── requirements.txt
├── README.md
│
└── models/
    └── best_model_full.pth
```

### Main Files

**app.py**  
Runs the Streamlit user interface.

**pipeline.py**  
Handles the machine learning prediction pipeline.

**utils.py**  
Contains supporting functions used by the application.

**requirements.txt**  
Lists the Python packages required to run the project.

**best_model_full.pth**  
Contains the trained PyTorch model.

## Installation

Clone the repository:

```bash
git clone https://github.com/NitNit-1738/brain-tumor-detection-ui.git
```

Move into the project directory:

```bash
cd brain-tumor-detection-ui
```

Install the required packages:

```bash
pip install -r requirements.txt
```

## Running the Application

Start the Streamlit application with:

```bash
streamlit run app.py
```

Streamlit should open the application in your web browser.

## Model Output

The model can predict the following classes:

| Class | Description |
|---|---|
| Glioma | MRI classified as a glioma tumor |
| Meningioma | MRI classified as a meningioma tumor |
| Pituitary Tumor | MRI classified as a pituitary tumor |
| No Tumor | MRI classified as showing no tumor |

The application also displays a confidence score to show how confident the model is in its prediction.

## Screenshots

Screenshots of the application can be added here to demonstrate the user interface and prediction results.

## Disclaimer

This project was created for educational and research purposes. The predictions produced by this application should not be considered a medical diagnosis. Medical images and results should be reviewed by qualified healthcare professionals.

## Author

**Cameron Askins**

Computer Science Student  
Georgia Southern University

GitHub: NitNit-1738
