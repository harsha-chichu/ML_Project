# ML_Project

## Overview

This repository contains a complete Machine Learning project pipeline — from data preprocessing and model training to deployment using Flask and AWS Elastic Beanstalk. The project demonstrates how to build, serve, and interact with a machine learning model via a web interface.

## Project Structure

```
ML_Project/
├── .ebextensions/         # AWS deployment configurations
├── artifacts/             # Saved models and data artifacts
├── catboost_info/         # Logs from CatBoost training
├── notebook/              # Jupyter notebooks for exploration
├── src/                   # Source code for pipeline
├── templates/             # HTML templates for web UI
├── application.py         # Flask app for model inference
├── requirements.txt       # Required Python packages
├── setup.py               # Install script
└── README.md              # Project description
```

## Features

- **Data Pipeline:** Structured modules for ingestion, transformation, and validation
- **Modeling:** CatBoost used for efficient and accurate training
- **Web App:** Flask-based interface for real-time predictions
- **AWS Deployment Ready:** Includes `.ebextensions` config for Elastic Beanstalk

## Getting Started

### Prerequisites

- Python 3.7 or later
- pip

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/harsha-chichu/ML_Project.git
   cd ML_Project
   ```

2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Run the Application

Start the Flask app locally:

```bash
python application.py
```

Then open your browser and visit: [http://localhost:5000](http://localhost:5000)

## Deployment (AWS Elastic Beanstalk)

To deploy on AWS:

1. Install EB CLI: https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-install.html
2. Initialize and deploy:
   ```bash
   eb init
   eb create your-env-name
   eb open
   ```

## Contributing

Feel free to fork this repository and submit pull requests. Suggestions and improvements are welcome!

## License

This project is licensed under the MIT License.
