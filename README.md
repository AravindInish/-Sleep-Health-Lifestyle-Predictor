# Sleep Health & Lifestyle Predictor

A machine learning project that predicts an individual's sleep disorder category using health and lifestyle factors such as age, occupation, sleep duration, stress level, BMI category, blood pressure, and daily activity. The project uses a deep learning model built in Python and is implemented in a Jupyter Notebook, with a Streamlit app for interactive prediction.

## Overview

Sleep quality and health are strongly influenced by everyday habits, work patterns, and physiological indicators. This project explores how lifestyle and health metrics can be used to classify sleep status into categories like:

- Insomnia
- Sleep Apnea
- None (No disorder detected)

The model is trained on a sleep health dataset and uses preprocessing, categorical encoding, and a neural network to make predictions.

## Project Goals

- Analyze sleep-related health and lifestyle data
- Build a predictive model for sleep disorder classification
- Visualize the dataset and model performance
- Provide a simple user interface for live predictions

## Dataset

The project uses the Sleep Health and Lifestyle Dataset, which includes features like:

- Gender
- Age
- Occupation
- Sleep Duration
- Quality of Sleep
- Physical Activity Level
- Stress Level
- BMI Category
- Blood Pressure
- Heart Rate
- Daily Steps
- Sleep Disorder

This dataset is downloaded via KaggleHub and then processed in the notebook for model training.

## Model and Approach

The notebook follows a complete ML workflow:

1. Load the dataset
2. Clean and preprocess the data
3. Split the data into training and testing sets
4. Engineer features such as systolic and diastolic blood pressure
5. Encode categorical variables
6. Train a deep learning classifier using TensorFlow/Keras
7. Evaluate the model using accuracy and classification metrics
8. Save the trained model and preprocessor for deployment

The final model achieved strong performance during evaluation, with test accuracy around 93.33%.

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook
- Streamlit
- KaggleHub

## Repository Contents

- `Sleep_Health_and_Lifestyle.ipynb` — main notebook containing dataset loading, preprocessing, model training, evaluation, and Streamlit app generation
- `README.md` — project overview and usage instructions

## Getting Started

### Prerequisites

Make sure you have Python 3.9+ installed.

Install the required packages:

```bash
pip install pandas numpy scikit-learn tensorflow kagglehub streamlit
```

## Running the Notebook

Open `Sleep_Health_and_Lifestyle.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab and run all cells.

The notebook will:

- download the dataset
- preprocess the data
- train the model
- save model artifacts (`sleep_model.keras`, `preprocessor.pkl`, and `target_encoder.pkl`)
- generate a `app.py` file for the Streamlit interface

## Running the Streamlit App

After training the model, run:

```bash
streamlit run app.py
```

This will launch the interactive dashboard where users can input lifestyle and health values and receive a predicted sleep disorder category.

## Example Features Used in Prediction

The application accepts inputs such as:

- Gender
- Age
- Occupation
- Sleep duration
- Sleep quality score
- Physical activity level
- Stress level
- BMI category
- Heart rate
- Daily steps
- Blood pressure

## Project Highlights

- End-to-end machine learning workflow
- Deep learning-based sleep disorder prediction
- User-friendly Streamlit interface
- Focus on health analytics and preventive wellness monitoring

## Future Improvements

- Add more sleep-related features and demographic data
- Compare multiple model architectures
- Add visual analytics and explainability dashboards
- Deploy the app online using Streamlit Cloud or Hugging Face Spaces

## License

This project is available for educational and research purposes. Please check the repository license if one is added later.

## Author

AravindInish

## Note

This repository is designed as a practical data science and AI project focused on sleep health prediction. It is ideal for learning data preprocessing, model training, classification, and deployment workflows.
