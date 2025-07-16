# Plant-Disease-Recognition-System-Using-Machine-Learning
Plant-Disease-Recognition-System-Using-Machine-Learning

# 🌿 Plant Disease Recognition System Using Machine Learning

This project uses deep learning and computer vision to detect plant diseases from leaf images. A TensorFlow-based model is integrated with a Flask web application for a simple and intuitive interface that allows users to upload plant leaf images and get a prediction with possible causes and cures.

---

## 📁 Repository Structure

Plant-Disease-Recognition-System-Using-Machine-Learning/
│
├── app.py # Flask app
├── plant_disease.json # Metadata with disease name, cause, and cure
├── model_download.txt # Model download link
├── models/ # Folder for the Keras model
│ └── plant_disease_recog_model_pwp.keras
├── static/ # CSS, JS, and image assets
│ └── css/
│ └── js/
├── templates/ # HTML templates
│ └── home.html
├── uploadimages/ # Temporarily stores uploaded images
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🧠 Model Details

- **Framework**: TensorFlow / Keras
- **Input**: Leaf images (160x160)
- **Output**: Predicted plant disease name, cause, and cure
- **Classes**: Trained on 38 different disease/healthy leaf categories

---

## 🚀 How It Works

1. User uploads a leaf image.
2. The model processes the image and predicts the disease class.
3. Flask displays:
   - The uploaded image
   - Disease name
   - Cause
   - Cure

---

## 🔧 Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/vksharma3010/Plant-Disease-Recognition-System-Using-Machine-Learning.git
cd Plant-Disease-Recognition-System-Using-Machine-Learning
2. Create a Virtual Environment (recommended)
bash
Copy
Edit
conda create -n plant-env python=3.10 -y
conda activate plant-env
3. Install Dependencies
bash
Copy
Edit
conda install tensorflow -y
pip install flask numpy
4. Download the Model
Download the trained model from the link in model_download.txt and place it inside the models/ folder.

▶️ Run the App
bash
Copy
Edit
python app.py
Visit: http://127.0.0.1:5000 in your browser.

📸 Sample UI

📄 Dataset
The model is trained on a publicly available PlantVillage Dataset containing thousands of leaf images across various plant species and diseases.


