# 🌿 MediScan AI
### Intelligent Medicinal Plant Identification Using Deep Learning

MediScan AI is an AI-powered medicinal plant identification system that uses computer vision and deep learning to recognize medicinal plants from leaf images. It provides an accessible platform for image-based plant classification, helping users explore medicinal plant information through an intuitive web application.

The system integrates a Python Flask backend with a PyTorch-based deep learning model to generate plant predictions, confidence scores and relevant botanical information.

## ✨ Key Features

- **AI-Based Plant Recognition:** Identifies medicinal plants using uploaded leaf images.
- **Deep Learning Classification:** Uses a fine-tuned ResNet50 architecture.
- **30 Plant Categories:** Recognizes 30 medicinal plant classes.
- **Confidence Estimation:** Displays the model's prediction confidence.
- **Plant Information:** Presents descriptions of identified medicinal plants.
- **Image Preview:** Allows users to preview images before classification.
- **Responsive Interface:** Supports desktop and mobile devices.
- **Optimized Inference:** Designed for efficient CPU-based model execution.
- **Integrated Application:** Combines image processing, classification and result presentation in one web application.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python, Flask |
| Deep Learning | PyTorch |
| Model Architecture | ResNet50 |
| Image Processing | Pillow, torchvision |
| Production Server | Gunicorn |
| Version Control | Git, GitHub |

## 🧠 System Architecture

```text
           USER
             |
             v
       WEB INTERFACE
             |
             v
        IMAGE UPLOAD
             |
             v
       FLASK BACKEND
             |
             v
     IMAGE PREPROCESSING
             |
             v
     DEEP LEARNING MODEL
          RESNET50
             |
             v
      CLASSIFICATION
             |
       +-----+------+
       |     |      |
       v     v      v
      Plant Confidence Plant
      Name  Score    Information
       |     |      |
       +-----+------+
             |
             v
       RESULT DISPLAY
```

## 📁 Project Structure

```text
MediScan-AI/
│
├── app.py
├── inference.py
├── requirements.txt
├── gunicorn.conf.py
├── Dockerfile
├── .gitignore
│
├── model/
│
├── data/
│
├── templates/
│   ├── index.html
│   └── result.html
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── tests/
│
└── README.md
```

## 🚀 Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/MediScan-AI.git
cd MediScan-AI
```

### 2. Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the trained model

Place the trained model checkpoint in the configured model directory or follow the repository's model download instructions.

Ensure that the model architecture, preprocessing configuration and class mapping match the trained checkpoint.

### 5. Start the application

```bash
python app.py
```

Open:

```text
http://127.0.0.1:5000
```

## ⚙️ Working Process

1. The user accesses the web application.
2. A leaf image is uploaded through the interface.
3. The backend validates and preprocesses the image.
4. The trained deep learning model performs classification.
5. The predicted plant category is identified.
6. The corresponding confidence score and plant information are retrieved.
7. The classification results are displayed to the user.

## 📊 Model Specifications

| Parameter | Details |
|---|---|
| Model Architecture | ResNet50 |
| Framework | PyTorch |
| Learning Task | Image Classification |
| Classification Categories | 30 |
| Input | Medicinal plant leaf images |
| Output | Plant category and confidence |
| Inference | CPU-compatible |

## ⚡ Performance Optimization

The system is designed with deployment efficiency in mind.

Optimization objectives include:

- Single-time model initialization.
- Reduced dependency overhead.
- Efficient image preprocessing.
- CPU-based inference.
- Model checkpoint optimization.
- Reduced runtime memory consumption.
- Removal of unnecessary training components.

## 🔒 Security and Reliability

- Image format validation.
- Upload size restrictions.
- Secure file handling.
- Temporary file cleanup.
- Error handling.
- Environment-based configuration.
- Production-ready application serving.

## 🌐 Deployment

The application is structured for deployment on Python-compatible hosting platforms.

Deployment configuration includes:
- Gunicorn application serving.
- CPU-based model inference.
- Configurable application ports.
- Model storage configuration.
- Health-check endpoint.

Hosting availability and performance depend on the selected provider's resource limits.

## 🎯 Project Vision

To make medicinal plant identification more accessible through intelligent image recognition, combining deep learning, computer vision and a simple digital experience.

## ⚠️ Disclaimer

This application is intended for educational and informational purposes. Predictions are not guaranteed to be botanically accurate and must not be used as a substitute for professional botanical identification or medical advice.

## 📜 License

Specify the applicable license after verifying the ownership and licensing of all code, model weights, datasets and other included resources.
