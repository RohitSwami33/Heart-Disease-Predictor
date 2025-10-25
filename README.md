


# Heart Disease Predictor

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)

A machine learning application designed to predict the likelihood of a patient having heart disease based on various clinical and demographic attributes. This project leverages a dataset of patient data to train a classification model, which is then served through an interactive web interface built with Streamlit.

## 🎯 Project Overview

Heart disease is a leading cause of mortality worldwide. Early detection and risk assessment are critical for effective prevention and treatment. This project aims to provide a simple, accessible tool that can assist in preliminary risk assessment by analyzing key health indicators.

The model takes inputs such as age, sex, chest pain type, blood pressure, cholesterol levels, and other relevant medical data to output a prediction on whether the patient is likely to have heart disease.

## ✨ Features

-   **Interactive Web Interface**: A user-friendly Streamlit application for easy input of patient data.
-   **Real-time Prediction**: Get instant predictions based on the trained machine learning model.
-   **Data Visualization**: Visualize key data distributions and correlations.
-   **Model Information**: View details about the model used and its performance metrics.
-   **Responsive Design**: Works seamlessly on both desktop and mobile devices.

## 🚀 Installation and Setup

To get this project up and running on your local machine, follow these steps:

### Prerequisites

-   Python 3.8 or higher
-   `pip` (Python package installer)

### Steps

1.  **Clone the repository**
    ```bash
    git clone https://github.com/RohitSwami33/Heart-Disease-Predictor.git
    ```

2.  **Navigate to the project directory**
    ```bash
    cd Heart-Disease-Predictor
    ```

3.  **Create a virtual environment** (Recommended)
    ```bash
    # For macOS/Linux
    python3 -m venv venv
    source venv/bin/activate

    # For Windows
    python -m venv venv
    .\venv\Scripts\activate
    ```

4.  **Install the required dependencies**
    ```bash
    pip install -r requirements.txt
    ```

## 🖥️ Usage

Once the installation is complete, you can run the Streamlit application.

1.  **Run the app**
    ```bash
    streamlit run app.py
    ```

2.  **Open your web browser**
    Navigate to the local URL provided in the terminal (usually `http://localhost:8501`).

3.  **Use the application**
    Enter the patient's details in the sidebar and click the "Predict" button to see the result.

## 📁 Project Structure

```
Heart-Disease-Predictor/
├── data/
│   └── heart_disease.csv       # The dataset used for training
├── model/
│   └── heart_disease_model.pkl # The trained machine learning model
├── notebooks/
│   └── EDA_and_Modeling.ipynb  # Jupyter notebook for exploration and training
├── app.py                      # The main Streamlit application file
├── requirements.txt            # List of Python dependencies
└── README.md                   # This file
```

## 🤖 Model & Methodology

-   **Dataset**: The project uses the [Heart Disease UCI dataset](https://archive.ics.uci.edu/ml/datasets/heart+disease), a classic dataset for machine learning.
-   **Model**: A `Logistic Regression` model was chosen for its interpretability and good performance on this type of binary classification problem.
-   **Performance**: The model achieved an accuracy of approximately **85%** on the test set. Other metrics like precision, recall, and F1-score were also considered during evaluation.

## 📊 Dataset

The dataset contains 14 attributes, including:
-   `age`: Age in years
-   `sex`: (1 = male; 0 = female)
-   `cp`: Chest pain type
-   `trestbps`: Resting blood pressure (in mm Hg)
-   `chol`: Serum cholestoral in mg/dl
-   `fbs`: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
-   ...and more.

The target variable is `target`, which indicates the presence of heart disease (1 = disease, 0 = no disease).

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

## 👨‍💻 Author

**Rohit Swami**

-   GitHub: [@RohitSwami33](https://github.com/RohitSwami33)

---

**Note**: Remember to create a `requirements.txt` file in your repository with the necessary packages (e.g., `streamlit`, `pandas`, `scikit-learn`, `numpy`). If you don't have one, you can generate it by running `pip freeze > requirements.txt` in your activated virtual environment.
