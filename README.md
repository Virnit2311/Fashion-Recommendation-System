# Fashion-Recommendation-System 👗🧥

## Overview
StyleMate is an AI-powered fashion recommendation system that suggests visually similar fashion items from a curated dataset of over 44k images. Upload a fashion image and instantly receive 5 matching styles using deep learning and image similarity.

## Features
✔️ Upload any fashion-related image (tops, jeans, dresses, etc.)

✔️ Instantly get 5 closest matching images based on visual similarity

✔️ Powered by ResNet50 feature extraction and K-Nearest Neighbors (KNN)

✔️ Fast and lightweight Streamlit web app

✔️ Clean, responsive, and user-friendly interface

## How It Works
🔹 Feature Extraction:
A pre-trained ResNet50 model (without top layers) extracts high-level features from the uploaded image.

🔹 Similarity Matching:
Using K-Nearest Neighbors (KNN) with Euclidean distance, StyleMate finds the 5 most visually similar images from the dataset.

🔹 Display Results:
Results are displayed side-by-side for easy exploration and selection.

## Tech Stack
🛠️ Python

🛠️ TensorFlow / Keras

🛠️ Streamlit

🛠️ Scikit-learn

🛠️ OpenCV, PIL

🛠️ NumPy, Pandas

## Setup Instructions
📂 Clone the repository:
git clone <repository-link>
cd StyleMate

📦 Install the required packages:
pip install -r requirements.txt

🗂️ Make sure the following files are present:
🔹embeddings.pkl (precomputed feature vectors)

🔹filenames.pkl (corresponding filenames)

🔹styles.csv (optional: dataset metadata)

🔹Image dataset under appropriate folder (or adjust paths)

🚀 Run the application:
streamlit run main.py

🖼️ Upload a fashion image and enjoy the recommendations!

## File Structure

├── app.ipynb           # Notebook for experimentation
├── main.py             # Main Streamlit application
├── styles.csv          # Dataset metadata
├── filenames.pkl       # Filenames for dataset images
├── embeddings.pkl      # Precomputed image features
├── uploads/            # Directory for uploaded images
├── README.md           # Project documentation

## Future Improvements
✨ Add category-based filtering (tops, bottoms, dresses, etc.)

✨ Include user preference learning for smarter suggestions

✨ Deploy on cloud platforms (AWS, Streamlit Cloud, Heroku)

## Acknowledgements
🔹ResNet50 - Keras Applications

🔹Streamlit

🔹Dataset source (custom dataset or public like DeepFashion)
