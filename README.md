# 🩺 Healthcare Chatbot

An intelligent command-line chatbot that interacts with users, asks about symptoms, and predicts possible diseases using machine learning models. It also provides descriptions and precautionary measures to improve health awareness and assist in early diagnosis.

---

## 📌 Problem Statement

Many individuals face delays in consulting healthcare professionals due to lack of awareness or accessibility. There is a growing need for an automated system that can offer preliminary health analysis based on symptoms and recommend precautions before professional consultation.

---

## ✅ Features

- Accepts user symptoms via interactive CLI
- Uses machine learning (Decision Tree & SVM) to predict possible diseases
- Provides disease descriptions and severity analysis
- Offers precautionary suggestions for the user
- Optional text-to-speech output using `pyttsx3`
- Pattern-matching for partial or misspelled symptom inputs
- Simple and intuitive interface

---

## 🚀 How It Works

1. User enters symptoms.
2. The system searches and confirms the exact symptom using pattern matching.
3. It uses a trained Decision Tree to predict the disease.
4. A secondary SVM model confirms the result.
5. The chatbot displays:
   - Predicted disease(s)
   - Description of the disease(s)
   - Precautionary steps
   - Severity evaluation based on symptom duration

---

## 🛠️ Technologies Used

| Component         | Technology        |
|------------------|-------------------|
| Programming Lang | Python            |
| ML Models        | Decision Tree, SVM|
| Libraries        | `scikit-learn`, `pandas`, `pyttsx3`, `numpy` |
| Interface        | Command Line      |
| Data Format      | CSV files         |

---

## 🧠 Algorithm

- **Decision Tree Classifier**: Main model used for disease prediction based on symptoms.
- **Support Vector Machine (SVM)**: Secondary model to verify prediction accuracy.
- **Pattern Matching**: Uses regex to match user-entered symptom with dataset.

---

## 📂 Dataset Files

| File Name                  | Purpose                              |
|---------------------------|--------------------------------------|
| `Training.csv`            | Main training dataset                |
| `Testing.csv`             | Testing dataset                      |
| `symptom_Description.csv` | Maps diseases to brief descriptions |
| `symptom_precaution.csv`  | Lists precautions per disease       |
| `Symptom_severity.csv`    | Severity scores of each symptom     |

---

## 📷 Sample Output

