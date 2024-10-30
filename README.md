# Model Training and Testing Guide

## Prerequisites

1. **Python 3.9**: Ensure Python 3.9 is installed.

   - Install it via:
     ```bash
     sudo apt update
     sudo apt install python3.9
     sudo apt install python3.9-venv
     ```

2. **Virtual Environment Setup**: Set up a virtual environment for isolated package management.

   ```bash
   python3.9 -m venv obd
   source obd/bin/activate
   ```

---

## How to Train the Model Using Teachable Machine

1. **Collect Data**:

   - Use the `data_collect.py` script to collect images.
   - Organize collected images into separate folders for each class (e.g., folder A for "A" samples, folder B for "B" samples, etc., up to Z if needed).

2. **Teachable Machine Setup**:

   - Go to [Teachable Machine](https://teachablemachine.withgoogle.com/).
   - **Select the "Audio" Section** if training for audio classification (or "Image" if your project focuses on image recognition).
   - Define your classes (e.g., A, B, C, ... Z) to represent the different categories you want to classify.

3. **Train the Model**:

   - Upload your dataset into the Teachable Machine interface or record audio samples directly on the site.
   - Train your model by following the steps on Teachable Machine until you reach the export options.

4. **Export the Model**:

   - Once training is complete, export your model in the **TensorFlow** format.

5. **Download and Integrate**:
   - Download the model files (such as `saved_model.pb` and the variables folder).
   - Place the model in your project directory for easy access during testing.

---

**Update**:
Train Model: data_collect.py
Test Model: Testing.py

- As you Train the model both Python Files need to update about the model and its label configs

**Warning**: IT MAY POSSIBLE THAT requirements.txt FILE WOULD NOT WORK
