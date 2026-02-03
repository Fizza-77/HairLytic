# HairLytic
AI-Based Alopecia Detection Using YOLOv8

HairLytic is an end-to-end AI-powered computer vision application designed to assist in identifying common alopecia conditions from scalp images. It leverages a CNN-based YOLOv8 model, trained on a custom dataset, to classify images into three alopecia types:

Alopecia Areata

Alopecia Totalis

Androgenetic Alopecia

The application provides a web interface where users can upload images or capture them using their device camera, receive predictions, and track their prediction history over time.

Tech Stack
AI / Machine Learning

YOLOv8 (CNN-based object detection & classification)

Python

Backend

Flask (REST API)

Python

Frontend

React (Web UI)

Data Storage

Server-side image storage

Prediction history with timestamps

How It Works

User uploads a scalp image or captures one via the camera.

The image is sent to the Flask backend through a REST API.

The YOLOv8 model performs inference on the image.

The predicted alopecia type is returned and stored.

Users can view past predictions through the history dashboard.

Model Details

Architecture: YOLOv8 (CNN-based)

Training: Custom-curated alopecia dataset

Task: Multi-class classification for medical image analysis

Model weights are not included in this repository due to size constraints.

Model Training

In runs folder you may find the matrices and training set images along with best and last weights.

Environment Setup
Prerequisites

Python 3.8+

Node.js & npm

Virtual environment (recommended)

Backend Setup
cd backend
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt

Frontend Setup
cd frontend
npm install
npm start

Key Features

AI-driven alopecia classification using YOLOv8

Image upload and real-time camera capture

Prediction history tracking

Modular frontend-backend architecture

Scalable API design
