# AI Student Placement Prediction

## 📌 Project Overview

**AI Student Placement Prediction** is a machine learning project that predicts whether a student is likely to be placed based on academic performance, attendance, aptitude, programming ability, communication skills, and internship experience.

The project is implemented in Python and developed/run using JupyterLab. The notebook uses Pandas, NumPy, Scikit-learn, TensorFlow, and Matplotlib.

> **Note:** The uploaded HTML files are saved JupyterLab views. Although some uploaded filenames contain "cancer detection", the actual notebook content identifies the project as **AI Student Placement Prediction**.

## 🎯 Objective

The main objective is to build a binary classification model that predicts the student's placement status:

- `0` → Not placed
- `1` → Placed

The model uses the following student attributes:

- CGPA
- Attendance
- Aptitude score
- Programming score
- Communication score
- Internship status

## 🛠️ Technologies Used

- **Python**
- **Pandas** – data loading and manipulation
- **NumPy** – numerical operations
- **Scikit-learn** – data splitting, scaling, and evaluation
- **TensorFlow / Keras** – neural network model
- **Matplotlib** – visualization
- **JupyterLab** – development environment

## 📊 Dataset

The code loads the dataset from:

```text
student_data.csv
```

The input features are:

```text
CGPA
Attendance
Aptitude
Programming
Communication
Internship
```

The target column is:

```text
Placement
```

The uploaded notebook output shows sample records containing these fields and a binary `Placement` value.

## 🔄 Project Workflow

The project follows these main steps:

1. Import the required Python libraries.
2. Load `student_data.csv` using Pandas.
3. Separate input features (`X`) and target (`y`).
4. Split the data into training and testing sets.
5. Standardize the input features using `StandardScaler`.
6. Build a TensorFlow/Keras neural network.
7. Train the model for 50 epochs with a batch size of 4 and a validation split of 20%.
8. Evaluate the model using test accuracy.
9. Generate predictions.
10. Convert prediction probabilities to binary classes using a `0.5` threshold.
11. Generate an accuracy score, classification report, and confusion matrix.
12. Use the trained model to predict whether a student is likely to be placed.

## 🧠 Model Training

The project uses a neural-network-based classification model implemented with TensorFlow/Keras.

The training configuration shown in the notebook is:

- **Epochs:** 50
- **Batch size:** 4
- **Validation split:** 20%
- **Evaluation metric:** Accuracy

The notebook also applies feature scaling before model training.

## 📈 Model Evaluation

The project evaluates the model using:

- Accuracy
- Classification Report
- Confusion Matrix

The recorded classification report shows:

| Class | Precision | Recall | F1-score | Support |
|------:|----------:|-------:|---------:|--------:|
| 0 | 0.99 | 1.00 | 0.99 | 88 |
| 1 | 1.00 | 0.92 | 0.96 | 12 |

The recorded test accuracy is **0.99 (99%)**.

The confusion matrix shown in the notebook is:

```text
[[88, 0],
 [ 1, 11]]
```

## 🔮 Prediction

After training and evaluation, the project performs prediction on student data.

The recorded example output is:

```text
Prediction : Student is likely to be PLACED
```

## 🚀 How to Run

### 1. Install Python

Make sure Python is installed on your system.

### 2. Install the required packages

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow jupyterlab
```

### 3. Place the dataset

Keep the dataset file in the same working directory as the notebook:

```text
student_data.csv
```

### 4. Open JupyterLab

```bash
jupyter lab
```

### 5. Open the notebook

Open the project notebook in JupyterLab and run the cells from top to bottom.

## 📁 Suggested Project Structure

```text
AI-Student-Placement-Prediction/
│
├── student_data.csv
├── placement_prediction.ipynb
├── README.md
└── requirements.txt
```

## ⚠️ Limitations

- The prediction depends on the quality and representativeness of the training dataset.
- A high test accuracy does not guarantee correct predictions for every new student.
- The model should be treated as a prediction/educational tool rather than a replacement for real-world placement decisions.
- The uploaded notebook records a TensorFlow warning about GPU support on native Windows; CPU execution can still be used.

## 🔮 Future Improvements

Possible improvements include:

- Use a larger and more diverse student dataset.
- Compare multiple classification algorithms.
- Add cross-validation.
- Tune neural-network hyperparameters.
- Add more student-related features.
- Build a simple web interface for entering student details.
- Save and load the trained model for future predictions.
- Add charts for feature analysis and model performance.

## 📚 Project Learning Outcomes

This project demonstrates practical experience with:

- Data preprocessing
- Feature selection
- Train-test splitting
- Feature scaling
- Neural-network classification
- Model training and validation
- Prediction
- Classification metrics
- Confusion-matrix analysis
- Python-based machine learning workflows

## 👤 Author

**AI Student Placement Prediction Project**

---

### Disclaimer

This project is intended for educational and demonstration purposes. Placement predictions should not be considered guaranteed outcomes.
