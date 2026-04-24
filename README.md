# Emotion_Aware_Product_Recommendation_System
Here’s a **clean, professional GitHub README.md** tailored for your project. You can copy-paste this directly into your repo.

---

# 📘 Emotion-Aware Product Recommendation System

An AI-powered system that analyzes user text to detect **emotion** and **emotion intensity**, and recommends relevant products using a real-world e-commerce dataset.

---

## 🚀 Overview

This project combines:

* 🧠 **Emotion Classification (NLP + Deep Learning)**
* 📊 **Emotion Intensity Prediction (Regression)**
* 🛒 **Product Recommendation System**

The system takes user text as input and outputs:

* Predicted Emotion
* Emotion Intensity (0–1)
* Recommended Products (based on emotion)

---

## 🧠 System Pipeline

```
User Text
   ↓
Tokenizer
   ↓
Emotion Classification Model
   ↓
Emotion Intensity Regression Model
   ↓
Emotion → Category Mapping
   ↓
Product Recommendation (Flipkart Dataset)
```

---

## 📂 Project Structure

```
├── models/
│   ├── emotion_classification_model.h5
│   ├── emotion_intensity_regression_model.h5
│
├── encoders/
│   ├── tokenizer.pkl
│   ├── labelencoder.pkl
│
├── data/
│   ├── processed_flipkart_products.csv
│
├── notebooks/
│   ├── training_notebook.ipynb
│   ├── inference_notebook.ipynb
│
├── app/
│   ├── gradio_app.py
│
├── README.md
```

---

## 📊 Datasets Used

### 1️⃣ GoEmotions Dataset

* Multi-class emotion classification
* 27 emotion labels

### 2️⃣ NRC Emotion Intensity Dataset

* Provides emotion intensity scores (0–1)
* Used for regression

### 3️⃣ Flipkart Product Dataset

* Real-world e-commerce data
* Cleaned and normalized categories

---

## ⚙️ Models Used

### 🔹 Emotion Classification Model

* Embedding Layer
* Bidirectional LSTM
* Dropout
* Dense (ReLU)
* Output (Softmax)

---

### 🔹 Emotion Intensity Regression Model

* Embedding Layer
* LSTM
* Dropout
* Dense (ReLU)
* Output (Linear)

---

## 🔧 Technologies Used

* Python
* TensorFlow / Keras
* NumPy, Pandas
* NLP Techniques
* Gradio (UI)

---

## 🧪 Example

**Input:**

```
I feel very lonely today
```

**Output:**

```
Emotion: sadness  
Intensity: 0.82  

Recommended Products:
- Home decor items  
- Beauty products  
- Stationery items  
```

---

## ▶️ How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/emotion-product-recommendation.git
cd emotion-product-recommendation
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Run Gradio App

```bash
python app/gradio_app.py
```

---

## 🧠 Key Features

* Emotion-aware recommendations
* Deep learning-based NLP models
* Real-world product dataset
* End-to-end pipeline
* Interactive UI using Gradio

---

## 📈 Evaluation Metrics

### Classification:

* Accuracy
* Precision
* Recall
* F1 Score

### Regression:

* MSE (Mean Squared Error)
* MAE (Mean Absolute Error)

---

## ⚠️ Limitations

* Rule-based emotion-category mapping
* No user personalization
* Limited dataset diversity

---

## 🚀 Future Work

* Use BERT / Transformers
* Personalized recommendations
* Real-time deployment
* User feedback integration

---

## 🤝 Contributing

Feel free to fork the repo and contribute improvements!


## 🙌 Acknowledgements

* GoEmotions Dataset (Google Research)
* NRC Emotion Intensity Dataset
* Flipkart Dataset

---

## 👨‍💻 Author

**Sanjiv Kumar**
**Giftson Raj**
**Mehanthika**
Data Science & AI Enthusiast
