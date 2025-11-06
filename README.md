# 🔒 Secure MFA System 🛡️

## Project Overview

This project is a robust, full-stack application that implements a **Multi-Factor Authentication (MFA)** system. It consists of a `Flask` backend that handles user authentication, password management, and core MFA logic, and a `Streamlit` frontend that provides a user-friendly interface for registration, login, and MFA setup. The system also integrates machine learning capabilities for advanced analysis, potentially for fraud detection or user behavior modeling.

This project is designed to enhance the security of user accounts by requiring a second form of verification beyond just a password.

***

## ✨ Features

* **User Authentication**: Secure user registration and login using industry-standard password hashing with `bcrypt`.
* **Multi-Factor Authentication**: Implements Time-based One-Time Passwords (TOTP) for MFA.
* **QR Code Generation**: Users can easily set up MFA by scanning a QR code with an authenticator app.
* **Interactive Frontend**: A dynamic and responsive user interface built with `Streamlit` and `streamlit-option-menu`.
* **Data Analysis Integration**: Includes libraries like `scikit-learn` and `imbalanced-learn`, hinting at advanced data processing or predictive modeling.
* **PDF Reporting**: The ability to generate PDF reports using `fpdf`, possibly for user data or transaction logs.
* **RESTful API**: A `Flask` backend with `Flask-Cors` support, providing a clean and secure API for the frontend.

***

## 🛠️ Technologies Used

* **Backend**:
    * 🐍 **Python**
    * 🌐 **Flask**: Web framework for the server.
    * 🔐 **bcrypt**: Password hashing library.
    * 🔑 **pyotp**: TOTP (MFA) implementation.
    * 🔄 **requests**: HTTP library for making API calls.
* **Frontend**:
    * 🚀 **Streamlit**: Application framework for the UI.
    * 📋 **streamlit-option-menu**: For creating navigation menus in Streamlit.
    * 📊 **pandas** & **numpy**: Data manipulation and analysis.
    * 🖼️ **qrcode**: QR code generation.
    * 📄 **fpdf**: PDF document creation.
* **Machine Learning**:
    * 🤖 **scikit-learn**: Machine learning library.
    * ⚖️ **imbalanced-learn**: For handling imbalanced datasets.

***

## 🚀 Installation & Setup

1.  **Clone the repository**:
    ```bash
    git clone <repository_url>
    cd <repository_folder>
    ```

2.  **Create a virtual environment** and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required libraries**:
    ```bash
    pip install -r requirements.txt
    ```

***

## 🏃 Usage

1.  **Start the Flask backend server**:
    ```bash
    python server.py
    ```

2.  **Open a new terminal** and start the Streamlit frontend:
    ```bash
    streamlit run client.py
    ```

3.  Access the application in your web browser at the provided `http://localhost:8501` address.
