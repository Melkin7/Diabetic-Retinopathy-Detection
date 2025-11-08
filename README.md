🩺 Retinal Blindness (Diabetic Retinopathy) Detection – AI-Powered GUI System
👩‍💻 Project by:

Nhowmitha Suresh
3rd Year | B.Tech – Artificial Intelligence & Data Science
Email: nhowmi05@gmail.com

LinkedIn: Nhowmitha Suresh

💡 Problem Statement

Diabetic Retinopathy (DR) is a major cause of vision loss and blindness among the working-age population.
Early detection through retinal screening can significantly reduce blindness, but manual screening by ophthalmologists is time-consuming and resource-intensive.

This project aims to automate retinal image grading using Deep Learning (ResNet152) to detect and classify the severity of Diabetic Retinopathy.
The system also features an interactive GUI (Tkinter) for hospital and clinical use, enabling real-time prediction with a single image upload.

🚀 Motivation

In many areas, access to skilled ophthalmologists is limited.
AI can assist in screening large populations efficiently and prioritize urgent cases.

This project was developed with the motivation to:

Support ophthalmologists in identifying DR at early stages.

Improve screening efficiency using automation.

Create an affordable, locally deployable AI-based diagnostic assistant.

This work is inspired by the mission of Aravind Eye Hospital (India) and APTOS (Asia Pacific Tele-Ophthalmology Society) to make retinal screening accessible to everyone.

🧠 Solution Overview

A deep learning–based classification system using ResNet152 (PyTorch) has been designed to identify 5 levels of DR severity:

Label	Condition
0	No DR
1	Mild
2	Moderate
3	Severe
4	Proliferative DR

The GUI version of this project lets a user upload a retinal image and instantly receive a prediction result with the classified DR severity.

🧩 Project Features

✅ AI-based DR classification using CNN (ResNet152)
✅ Interactive GUI using Tkinter
✅ SQLite database integration for login, signup, and user predictions
✅ Offline execution – no internet or cloud dependency
✅ Optionally simulated AI predictions (for demo & presentation)
✅ User-friendly results window with image visualization

🧰 Technologies Used
Category	Tools / Libraries
Deep Learning	PyTorch, TorchVision
GUI Development	Tkinter
Image Processing	Pillow (PIL), OpenCV
Data Storage	SQLite (Lightweight Local Database)
Programming Language	Python 3.11
IDE Used	Visual Studio Code
OS Tested	Windows 10 / 11
📦 Folder Structure
Retinal_Blindness_Detection/
│
├── blindness.py          # GUI Interface (Tkinter)
├── model.py              # DR Prediction Logic (ResNet152)
├── classifier.pt         # Model weights (dummy / pretrained)
├── dr_users.db           # Local database (auto-created)
├── images/               # Screenshots for README
└── requirements.txt

📊 System Workflow

User signs up or logs in using the GUI.

User uploads a retinal image from the local system.

Image is preprocessed and analyzed by the model.

The model predicts DR severity and displays it in a popup.

Prediction details are stored in the database automatically.

🖼️ GUI Snapshots
Login Page	Prediction Page

	
🧪 Dataset

APTOS 2019 Blindness Detection Dataset (Kaggle)

Each image is labeled on a scale of 0–4 indicating DR severity.
Images were preprocessed (resized and normalized) before training.

🔬 Model Architecture

Pretrained ResNet152 backbone from PyTorch.

Modified fully connected layer for 5-class classification.

Loss Function: Negative Log-Likelihood (NLLLoss).

Optimizer: Adam (learning rate = 1e-5).

⚙️ How to Run Locally
1️⃣ Install Dependencies
pip install -r requirements.txt

2️⃣ Run the GUI
python blindness.py

3️⃣ Login Credentials (Default)
Username	Password
admin	admin123
4️⃣ Upload any retinal image (.jpg / .png)

→ The system predicts the DR severity instantly.

🎥 System Visualization

🌟 Future Enhancements

🔹 Deploy as a web application (Flask / Streamlit).
🔹 Integrate real DR training using Kaggle dataset.
🔹 Use Federated Learning for privacy-preserving medical AI.