## End to End Machine Learning Project
# Student Performance Prediction

A machine learning web application that predicts a student's mathematics score based on demographic, socioeconomic, and academic attributes. The project demonstrates a complete end-to-end ML workflow, from data preprocessing and model training to deployment using Flask, Docker, and AWS.

---

## Features

- End-to-end machine learning pipeline
- Data preprocessing and feature engineering
- Model training and evaluation
- Interactive web interface for predictions
- Dockerized application
- Deployable on AWS Elastic Beanstalk

---

## Tech Stack

- Python
- Scikit-learn
- Pandas
- NumPy
- Flask
- Docker
- AWS Elastic Beanstalk

---

## Project Structure

```
student-performance/
│
├── artifacts/             # Trained model and preprocessing pipeline
├── notebook/              # Jupyter notebooks and experimentation
├── src/                   # Source code
│   ├── components/
│   ├── pipeline/
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── templates/             # HTML templates
├── static/                # CSS/JS assets
├── app.py                 # Flask application
├── requirements.txt
├── Dockerfile
├── setup.py
└── README.md
```

---

## Dataset

The project uses the **Student Performance** dataset containing information such as:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

The target variable is:

- **Mathematics Score**

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/venix7/student-perfomance.git

cd student-perfomance
```

### 2. Create a virtual environment

Windows

```bash
python -m venv venv
venv\Scripts\activate
```

Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Application

Start the Flask server.

```bash
python app.py
```

The application will start on

```
http://127.0.0.1:5000
```

Open the URL in your browser and enter the required student details to generate a prediction.

---

## Running with Docker

### Build the Docker image

```bash
docker build -t student-performance .
```

### Run the container

```bash
docker run -p 5000:5000 student-performance
```

The application will be available at

```
http://localhost:5000
```

---

## Machine Learning Workflow

1. Data Collection
2. Data Validation
3. Data Preprocessing
4. Feature Engineering
5. Model Training
6. Model Evaluation
7. Model Serialization
8. Flask Integration
9. Docker Containerization
10. AWS Deployment

---

## Model Prediction

The application takes the following inputs:

- Gender
- Race/Ethnicity
- Parental Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

It predicts the expected **Mathematics Score**.

---

## Future Improvements

- Model monitoring
- CI/CD pipeline using GitHub Actions
- User authentication
- Prediction history
- Cloud database integration
- REST API endpoints
- Explainable AI (SHAP/LIME)

---

## Author

**Uday**

GitHub: https://github.com/venix7

LinkedIn: *(Add your LinkedIn profile here)*

---
## License

This project is licensed under the MIT License.
