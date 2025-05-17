
# 🚘 Vehicle Damage Detection using Deep Learning

This project is a **Streamlit web application** that predicts vehicle damage type from an image using a fine-tuned **ResNet50** model built with **PyTorch**.

---

## 🔍 Overview

Upload a car image and let the model classify it into one of six categories:

- Front Breakage  
- Front Crushed  
- Front Normal  
- Rear Breakage  
- Rear Crushed  
- Rear Normal

---

## 🧰 Tech Stack

- **Frontend:** Streamlit
- **Backend:** Python, PyTorch, Torchvision
- **Model:** Fine-tuned ResNet50
- **Image Processing:** PIL, Torchvision Transforms

---

## 🚀 Getting Started

### 1. Clone the repository

```
git clone https://github.com/your-username/vehicle-damage-detection.git
cd vehicle-damage-detection
````

### 2. Create a virtual environment

```
python -m venv venv
# Activate (Windows)
venv\Scripts\activate
# Activate (macOS/Linux)
source venv/bin/activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```

### 4. Run the Streamlit app

```
streamlit run Streamlit-app/app.py
```

> Make sure `saved_model.pth` is placed inside the `Streamlit-app` directory.

---

## 📂 File Structure

```
vehicle-damage-detection/
├── Streamlit-app/
│   ├── app.py
│   ├── model_helper.py
│   └── saved_model.pth
├── server.py
├── requirements.txt
└── README.md
```

---

## 🧠 Model Details

* Architecture: ResNet50 (pretrained)
* Modified FC layer with dropout + 6-class output
* Layer4 and FC unfrozen for fine-tuning
* Input image size: 224x224

---

## 📸 Example

![Screenshot 2025-05-17 165824](https://github.com/user-attachments/assets/d3cc9754-9490-46e9-979d-6a57ec603a6d)


```
Predicted Class: Front Breakage
```

---

## 📝 Requirements

Core packages required:

* `streamlit`
* `torch`
* `torchvision`
* `Pillow`

(Full list in `requirements.txt`)

---

## 🙋 Author

**Parth Bijal Bharadia**
B.Tech CSE (Health Informatics) @ VIT Bhopal
GitHub: [ParthBharadia](https://github.com/ParthBharadia)

---
