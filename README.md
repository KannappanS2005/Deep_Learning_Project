# AR Dashboard Backend & Deep Learning Projects

Welcome to the **AR Dashboard Dataset** repository! This project is a comprehensive collection that serves a dual purpose: 
1. A **Flask Backend API** designed to provide data for an Augmented Reality (AR) Sales Dashboard.
2. A **Deep Learning Computer Vision Project** for Face Mask Detection using Convolutional Neural Networks (CNN).

## 🚀 Features

### 1. AR Sales Dashboard Backend
A robust Python-based API that processes sales and salary datasets to fuel a 3D/AR frontend interface.
* **RESTful API**: Exposes endpoints (`/api/person-data`) to fetch total and monthly salaries.
* **AR Data Generators**: Generates 3D grid sizes, AR position mappings (x, y, z coordinates), and color schemes for specific individuals.
* **KPI Computations**: Calculates total sales, top-performing individuals, and month-over-month growth rates.
* **Data Aggregation**: Utilizes `pandas` to group, aggregate, and process CSV datasets seamlessly.

### 2. Face Mask Detection (CNN)
An end-to-end Machine Learning Jupyter Notebook (`DL_Project_face_Mask_Detection_using_CNN.ipynb`).
* Uses **Deep Learning** and Convolutional Neural Networks to classify whether a person is wearing a face mask.
* Built for computer vision applications and public safety AI implementations.

## 🛠️ Technology Stack

* **Language**: Python 3.x
* **Backend Framework**: Flask, Flask-CORS
* **Data Science & ML**: Pandas, NumPy, Matplotlib
* **Environment Setup**: Pip (`requirements.txt`)
* **Deployment**: Configured for direct deployment on [Render](https://render.com/) via `render.yml`.

## 📂 Project Structure

```
.
├── DL_Project_face_Mask_Detection_using_CNN.ipynb  # CNN Face mask detection notebook
├── generate_charts.py                              # Utilities for AR 3D chart generation
├── render.yml                                      # Render deployment configuration
├── requirements.txt                                # Python dependencies
├── runtime.txt                                     # Python version specification
├── sales_data.csv                                  # Database/dataset for the AR dashboard
├── sales_model.py                                  # Data transformation and KPI logic
└── server.py                                       # Main Flask application entry point
```

## ⚙️ Local Setup and Installation

Follow these steps to run the Flask API locally on your machine:

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd AR_Dashboard_Datase-main
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Flask server:**
   ```bash
   python server.py
   ```
   The backend API will start running on `http://0.0.0.0:5000/`. You can access the data via `http://localhost:5000/api/person-data`.

## ☁️ Deployment

This project is fully configured for continuous deployment on **Render**. 
* The `render.yml` describes a web service named `ar-dashboard-nm`.
* It automatically installs the requirements and runs `python server.py`.
* To deploy, simply connect this repository to your Render account and it will deploy based on the YAML configuration file.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page or submit a Pull Request.

---
*Developed with ❤️ to empower AR data visualizations and AI/ML applications.*
