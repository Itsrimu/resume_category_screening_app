# Resume Screening Project

This project is a machine learning-based resume screening tool that classifies resumes into different categories using natural language processing (NLP) and supervised learning techniques.

## Project Structure

- `app.py`  
  Main application file (not shown in detail here).

- `resumeScreening.ipynb`  
  Jupyter notebook containing data analysis, feature extraction, model training, and prediction logic.

- `data/UpdatedResumeDataSet.csv`  
  Dataset containing resumes and their corresponding categories.

- `model/`  
  - `clf.pkl`: Trained classification model (e.g., SVM or Random Forest).
  - `encoder.pkl`: Label encoder for target categories.
  - `tfidf.pkl`: Trained TF-IDF vectorizer for text feature extraction.
- Just run  the wole NOTEBOOK after making model folder
## Features

- Loads and preprocesses resume data from CSV.
- Extracts features from resume text using TF-IDF vectorization.
- Trains a supervised classification model to predict resume categories.
- Saves trained models and encoders for later use.
- Provides a prediction function to classify new resumes.

## Usage

1. **Install dependencies**  
   Install required Python packages:
   ```
   pip install -r requirements.txt
   ```

2. **Run the notebook**  
   Open `resumeScreening.ipynb` in Jupyter Notebook or JupyterLab and run all cells to train the model and test predictions.

3. **Model Files**  
   After training, model files (`clf.pkl`, `encoder.pkl`, `tfidf.pkl`) are saved in the `model/` directory for reuse.

4. **Prediction**  
   Use the `pred` function in the notebook to predict the category of a new resume.


## Data

The dataset (`data/UpdatedResumeDataSet.csv`) should contain at least two columns:
- `Resume`: The text of the resume.
- `Category`: The target label for classification.

