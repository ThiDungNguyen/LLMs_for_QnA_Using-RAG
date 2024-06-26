This contain 3 sub-projects:
1. Word Correction using levenshtein_distance
2. Object Detection
3. Simple Chatbot
   

# Streamlit Project

This Streamlit application showcases various machine learning models and utilities. Its includes scripts for calculating Levenshtein distance, performing object detection with a MobileNet SSD model, and a simple chatbot implementation.

## Installation
1. Clone the repository:
```sh
git clone https://github.com/ThiDungNguyen/streamlit_examples.git
cd streamlit_example
```
2. (Optional) Create and activate a virtual environment:
```sh
python3 -m venv .pytorch
source .pytorch/bin/activate
```
3. Install the required dependencies:
```sh
pip install -r requirements.txt
```

## Running the Application
Once everything is ready, you can launch the application by running one of the following commands:
- [Levenshtein Distance Calculation](https://app-project-6q8qbsczuhh54nzt3xatcc.streamlit.app/)
```sh
streamlit run scripts/01_word_correction.py
```
- [Object Detection](https://app-project-br7kujv2xfmky84mbbzqvq.streamlit.app/)
```sh
streamlit run scripts/02_object_detection.py
```
- [Chatbot](https://app-project-v8ffadoqxud23vgymydvp3.streamlit.app/)
```sh
streamlit run scripts/03_chatbot.py
```