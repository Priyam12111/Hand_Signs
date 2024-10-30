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
   python3.9 -m venv my_env
   source my_env/bin/activate
   ```

3. **I trained my model from https://teachablemachine.withgoogle.com/**

---

## IT MAY POSSIBLE THAT requirements.txt FILE WOULD NOT WORK

# How To train the model

Prerequisite: Collect Images using data_collect.py FILE and Put it in different folder

1. Just go to website
2. Select Audio section
3. Mention all the classifier like A,B,C to Z
4. Download and integrate in Models Folder along with labels

---

Train Model: data_collect.py
Test Model: Testing.py
