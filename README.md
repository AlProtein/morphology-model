# Microalgae Morphology Detection

This repository provides a ready-to-use application for detecting and classifying microalgae (specifically, Spirulina) morphology in microscopic images using a deep learning model. It is tailored for R&D teams interested in quality assessment and research of microalgae strains.

## Overview

The application leverages a proprietary computer vision model to determine if uploaded microscopic images contain Spirulina. The tool is provided as a Streamlit web app, making it easy to use without deep technical knowledge.

- **Audience**: R&D teams, research groups, and labs working with microalgae.
- **Model**: A proprietary, pre-trained TensorFlow model (`spirulina_model.h5`) is included in this repository. The model will be updated as additional data becomes available and further development progresses.

## Features

- Upload single or multiple microscopic images for analysis.
- Detects and classifies images as Spirulina or not Spirulina.
- Adjustable confidence threshold for predictions.
- Downloadable report for each analysis.
- Keeps a history of predictions within the app session.

## Installation

1. **Clone this repository:**
   ```bash
   git clone https://github.com/AlProtein/morphology-model.git
   cd morphology-model
   ```

2. **Install required Python packages:**
   ```bash
   pip install -r requirements.txt
   ```

   The main requirements are:
   - streamlit
   - tensorflow
   - numpy
   - pandas
   - pillow

3. **Ensure the pre-trained model file `spirulina_model.h5` is present in the root directory.**  
   *(This is included in the repository. No training or download is required.)*

## Usage

1. **Start the Streamlit app:**
   ```bash
   streamlit run streamlit_app.py
   ```

2. **Open the provided local URL in your web browser.**

3. **Follow the on-screen instructions:**
   - Use the sidebar for information about the tool.
   - Set your desired confidence threshold.
   - Upload microscopic images (single or multiple) for classification.
   - Download result reports as needed.

## Example

After launching the app, you'll see:
- An "About" section with project details.
- Tabs for single and multiple image uploads.
- Prediction results and downloadable reports after analysis.

*No screenshots are provided in this README, but the UI is intuitive and self-explanatory.*

## Model Development

- The included model is proprietary and pre-trained for detection of Spirulina in microscopic images.
- Users are not expected to re-train the model.
- The model will be improved and updated in future releases as more labeled data is collected.

---

&copy; AlProtein, 2025. All rights reserved.
