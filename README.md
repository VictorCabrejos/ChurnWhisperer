<div align="center">

# 📊 ChurnWhisperer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect%20with%20Victor-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/victorcabrejos/)

## *Intelligent Customer Retention • AI-Powered Analytics • Telecom Solutions*

</div>

A modern web application for telecom customer churn prediction with AI explanations.

![ChurnWhisperer](app/static/images/logo.png)

## Overview

ChurnWhisperer is a sophisticated machine learning web application designed to predict customer churn in the telecommunications sector. By leveraging advanced algorithms and AI-powered explanations, it helps businesses understand and mitigate customer attrition risks.

## Features

- 🔮 **Advanced Prediction**: XGBoost model with SMOTE for handling imbalanced data
- 🧠 **AI Explanations**: Natural language explanations of predictions using GPT-4o-mini
- 📊 **Interactive Dashboard**: Visual representation of churn risks and metrics
- 💻 **Modern UI**: Futuristic and responsive user interface
- 🛠 **API Endpoints**: Full REST API for integration with other systems

## Tech Stack

- **Backend**: FastAPI, Python
- **Frontend**: Jinja2 Templates, HTML/CSS/JS, Bootstrap
- **ML**: XGBoost, scikit-learn, SMOTE
- **AI**: OpenAI GPT-4o-mini
- **Data Processing**: Pandas, NumPy
- **Visualization**: Chart.js

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/ChurnWhisperer.git
   cd ChurnWhisperer
   ```

2. Set up a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Configure your OpenAI API key in `config/settings.py`

5. Run the application:
   ```
   python run.py
   ```

6. Open your browser and go to `http://localhost:8000`

## Project Structure

```
ChurnWhisperer/
│
├── app/                      # Main application
│   ├── api/                  # API endpoints and services
│   │   └── prediction_service.py
│   ├── models/               # ML model implementations
│   │   └── model_trainer.py
│   ├── static/               # Static assets
│   │   ├── css/
│   │   ├── js/
│   │   └── images/
│   ├── templates/            # HTML templates
│   │   ├── base.html
│   │   ├── index.html
│   │   └── ...
│   ├── utils/                # Utility functions
│   └── main.py               # FastAPI application
│
├── config/                   # Configuration
│   └── settings.py
│
├── data/                     # Data files
│   └── churn.csv             # Telecom customer churn dataset
│
├── notebooks/                # Jupyter notebooks
│   └── ChurnWhisperer_Model_Training_and_Explanation.ipynb
│
├── requirements.txt          # Python dependencies
└── run.py                    # Application entry point
```

## Usage

1. **Landing Page**: Overview of ChurnWhisperer capabilities
2. **Dashboard**: View churn metrics and high-risk customers
3. **Prediction**: Submit customer data for churn prediction
4. **Results**: Get detailed prediction with AI explanation

## API Documentation

Once the application is running, visit `http://localhost:8000/docs` for interactive API documentation powered by Swagger UI.

### Main Endpoints:

- `POST /api/predict`: Predict churn for customer data
- `GET /api/dashboard`: Get dashboard statistics

## License

MIT License

## Acknowledgements

- Dataset: IBM Sample Data Sets
- Icons: Font Awesome
- UI Components: Bootstrap
