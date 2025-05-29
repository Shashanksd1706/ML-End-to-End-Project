## End to End Machine Learning Project
This project demonstrates the complete lifecycle of a machine learning application, from raw data preprocessing to model deployment with a user-friendly interface. It is designed to showcase practical experience in building scalable ML solutions with proper engineering practices.

📁 Project Structure
bash
Copy
Edit
ML-End-to-End-Project/
├── .github/workflows/         # CI/CD pipelines (GitHub Actions)
├── config/                    # Configuration schema and settings
├── notebook/                  # Jupyter notebooks for experimentation
├── src/                       # Core source code
├── templates/                 # Flask HTML templates
├── application.py             # Flask app entry point
├── requirements.txt           # Dependencies
├── setup.py                   # Installable package
├── Dockerfile                 # Docker configuration file
├── .dockerignore              # Docker ignore file
└── README.md                  # Project documentation
🔄 Workflow Overview
1. 📥 Data Ingestion
Reads raw CSV data from the source path.

Stores raw and split data (train/test) into structured folders.

Logs all data operations for reproducibility.

2. 🧹 Data Transformation
Cleans and preprocesses data.

Handles missing values, encodes categorical variables, and scales numerical features.

Saves the transformed dataset for model training.
DataCamp
+7
Machine Learning Models
+7
AmanXai
+7

3. 🤖 Model Training
Trains multiple machine learning models using scikit-learn.

Evaluates using metrics like accuracy, R², MAE, etc.

Selects and saves the best model using a custom evaluation pipeline.
ML Engineering Place
+1
Machine Learning Models
+1

4. 🧪 Model Evaluation
Validates model on test data.

Logs model performance, overfitting, and underfitting analysis.

5. 💾 Model Saving & Loading
Utilizes joblib for saving and loading models and transformers.

Ensures consistent preprocessing and predictions during deployment.
Dimitris Effrosynidis
+2
CertCommunity
+2
Machine Learning Models
+2

6. 🌐 Web Application (Flask)
A Flask-based UI to collect user inputs.

Passes inputs to the model and displays predictions.

Uses HTML templates in the templates/ folder.
AmanXai
+5
Dimitris Effrosynidis
+5
Machine Learning Models
+5

7. 🐳 Docker Containerization
Includes a Dockerfile to containerize the application.

Ensures consistency across different environments.

Facilitates easy deployment and scalability.
GeeksforGeeks

8. ☁️ Deployment on AWS
Application is deployed on AWS Elastic Beanstalk.

.ebextensions directory contains environment config.

Docker integration allows for seamless deployment.

9. ⚙️ CI/CD with GitHub Actions
Automated testing and deployment pipeline.

Ensures code quality and error-free deployments.

| Component        | Tools Used                  |
| ---------------- | --------------------------- |
| Language         | Python                      |
| ML Libraries     | scikit-learn, pandas, numpy |
| Web Framework    | Flask                       |
| Containerization | Docker                      |
| Deployment       | AWS Elastic Beanstalk       |
| Automation       | GitHub Actions              |
| Logging & Config | logging, configparser       |


# Clone the repository
git clone https://github.com/Shashanksd1706/ML-End-to-End-Project.git
cd ML-End-to-End-Project

# Build Docker image
docker build -t ml-end-to-end-project .

# Run Docker container
docker run -p 5000:5000 ml-end-to-end-project
