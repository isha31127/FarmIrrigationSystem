# Smart Sprinkler System 🌱💧

An AI-powered irrigation management system that predicts which sprinklers should be turned ON or OFF based on soil moisture sensor readings. The project uses Machine Learning to automate irrigation decisions, helping optimize water usage and improve farm efficiency.

## 📌 Project Overview

The Smart Sprinkler System uses data collected from 20 soil moisture sensors installed across a farm. A Machine Learning model analyzes these sensor values and predicts the irrigation status for different farm parcels.

The application provides a simple Streamlit-based web interface where users can enter sensor readings and instantly receive sprinkler activation recommendations.

---

## 🚀 Features

* Predicts sprinkler status for multiple farm parcels.
* Uses Machine Learning for intelligent irrigation decisions.
* Interactive web interface built with Streamlit.
* Real-time prediction based on sensor inputs.
* Water-efficient farming support.
* Easy-to-use slider-based input system.

---

## 🛠️ Technologies Used

* **Python**
* **Streamlit**
* **NumPy**
* **Pandas**
* **Scikit-learn**
* **Joblib**
* **Random Forest Classifier**
* **MultiOutputClassifier**

---

## 📂 Project Structure

```text
Smart-Sprinkler-System/
│
├── app.py                         # Streamlit web application
├── Farm_Irrigation_System.pkl     # Trained ML model
├── irrigation_machine.csv         # Dataset
├── Irrigation_System.ipynb        # Model training notebook
└── README.md
```

---

## 📊 Dataset Information

The dataset contains:

* **2000 records**
* **20 sensor features**

  * sensor_0 to sensor_19
* **3 target labels**

  * parcel_0
  * parcel_1
  * parcel_2

Each target label indicates whether the sprinkler for a specific parcel should be:

* **1 → ON**
* **0 → OFF**

---

## 🤖 Machine Learning Model

The model was trained using:

```python
RandomForestClassifier
```

wrapped inside:

```python
MultiOutputClassifier
```

This allows the system to predict irrigation requirements for multiple farm parcels simultaneously.

### Workflow

1. Load dataset
2. Data preprocessing
3. Feature scaling using MinMaxScaler
4. Train-test split
5. Model training
6. Performance evaluation
7. Model serialization using Joblib
8. Deployment with Streamlit

---

## ▶️ Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/smart-sprinkler-system.git

cd smart-sprinkler-system
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install streamlit numpy pandas scikit-learn joblib
```

---

## 🚀 Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 🖥️ How to Use

1. Launch the Streamlit application.
2. Adjust the sensor values using the sliders.
3. Click **Predict Sprinklers**.
4. View the predicted sprinkler status for each parcel.

Example Output:

```text
Sprinkler 0 (parcel_0): ON
Sprinkler 1 (parcel_1): OFF
Sprinkler 2 (parcel_2): ON
```

---

## 🌍 Applications

* Smart Agriculture
* Precision Farming
* Water Conservation
* Automated Irrigation Systems
* IoT-based Farming Solutions

---

## 🔮 Future Improvements

* Integration with real-time IoT sensors.
* Weather forecast-based irrigation recommendations.
* Mobile application support.
* Cloud deployment.
* Water consumption analytics dashboard.

---

## 👩‍💻 Author

**Isha Kumari**

MCA (AI & ML) Student
Uttaranchal University

---

## 📜 License

This project is developed for educational and research purposes. Feel free to use and modify it for learning and experimentation.
