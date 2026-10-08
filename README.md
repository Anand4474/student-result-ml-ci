# Student Result Prediction ML CI

Student Result Prediction machine-learning model with GitHub Actions CI.

## Features

- Reproducible dataset generation
- Logistic Regression classifier
- Accuracy and confusion matrix
- Saved model and metrics
- Automated ML tests
- GitHub Actions CI

## Input Features

- attendance
- internal_marks
- assignment_marks
- previous_score

## Target

- 1 = PASS
- 0 = FAIL

## Local Commands

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
python train_model.py
python -m unittest discover -v
```

## GitHub Actions

The workflow automatically:

1. Checks out the repository
2. Sets up Python 3.11
3. Installs ML dependencies
4. Generates the dataset
5. Trains and evaluates the model
6. Runs 7 automated tests

## Generated Files

The training program creates:

- student_results.csv
- student_result_model.pkl
- metrics.json
