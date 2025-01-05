# Crop Prediction System

## 🌟 Introduction

The **Crop Prediction System** is a web-based application designed to assist farmers and agricultural professionals in selecting the best crops for their specific soil and environmental conditions. Using a machine learning model trained on agricultural datasets, the system provides accurate crop recommendations, enhancing productivity and sustainability.

This project combines the power of Flask for backend development with an intuitive frontend built using HTML and CSS, delivering a user-friendly interface and robust functionality.

---

## ✨ Features

### User Features:
- **Input Form**: Enter parameters like Nitrogen, Phosphorus, Potassium, Temperature, Humidity, pH value, and Rainfall.
- **Crop Recommendation**: Predicts the most suitable crop based on the provided inputs.
- **Interactive Interface**: Simple and responsive design for easy use.

### Backend Features:
- **Machine Learning Integration**: Implements a Random Forest Classifier trained on agricultural data.
- **Dynamic Prediction**: Provides real-time predictions based on user input.
- **Scalability**: Designed to handle multiple users simultaneously.

---

## 🛠️ Technologies Used

- **Backend**: Python, Flask
- **Frontend**: HTML, CSS
- **Machine Learning**: Random Forest Classifier, Scikit-learn, Pandas, NumPy
- **Model Serialization**: Pickle
- **Visualization**: Matplotlib (for analysis during model development)

---

## 📂 Project Structure

```
CropPrediction
├── model.py                     # Machine learning model training and serialization
├── app.py                       # Flask application with routes for prediction
├── templates
│   └── index.html               # HTML template for the user interface
├── static                       # (Optional) Static assets for styles and images
├── Crop_recommendation.csv      # Dataset used for training the model
├── model.pkl                    # Serialized machine learning model
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

## 🚀 Installation

### 1. Clone the Repository
```bash
$ git clone https://github.com/yourusername/CropPrediction.git
$ cd CropPrediction
```

### 2. Set Up a Virtual Environment
```bash
$ python -m venv venv
$ source venv/bin/activate    # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
$ pip install -r requirements.txt
```

---

## ▶️ Run the Application

1. **Start the Flask Server**:
   ```bash
   $ flask run
   ```

2. **Access the Application**:
   Open your browser and navigate to `http://127.0.0.1:5000/`.

---

## 🌐 API Endpoints

### Prediction Endpoint
- **URL**: `POST /predict`
- **Request Body**:
  ```json
  {
    "Nitrogen": "value",
    "Phosphorus": "value",
    "Potassium": "value",
    "Temperature": "value",
    "Humidity": "value",
    "pH": "value",
    "Rainfall": "value"
  }
  ```
- **Response**:
  ```json
  {
    "Recommended Crop": "Crop Name"
  }
  ```

---

## 🔅 Deployment

### Prepare for Deployment
1. Ensure `requirements.txt` includes all dependencies.
2. Set environment variables for deployment platforms (e.g., Flask settings).

### Example Deployment on Heroku
```bash
$ heroku create
$ git push heroku main
$ heroku config:set FLASK_ENV=production
$ heroku open
```

---

## 📊 Dataset Description

The **Crop_recommendation.csv** dataset contains:
- **Features**: Nitrogen, Phosphorus, Potassium, Temperature, Humidity, pH, Rainfall
- **Target**: Crop name

The model is trained using these features to predict the most suitable crop for given conditions.

---

## 🤝 Contributing

Contributions are welcome! Follow these steps to contribute:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m 'Add feature-name'`.
4. Push to the branch: `git push origin feature-name`.
5. Submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 📱 Contact

For any queries or suggestions:
- **Email**: nishnatmishra7909@gmail.com
- **GitHub**: [Nishant123455](https://github.com/Nishant123455)

