# Evans Opande - Internal Medicine Expert AI

An AI-powered internal medicine assistant for symptom analysis, chronic disease risk prediction, lab result interpretation, and structured clinical report generation.

## Features

- Symptom analysis
- Disease risk prediction
- Lab result interpretation
- Patient history summarization
- Chronic illness monitoring
- Clinical report generation
- Streamlit dashboard
- FastAPI inference endpoint

## Tech Stack

- Python
- PyTorch / TensorFlow
- scikit-learn
- Pandas
- NumPy
- Hugging Face Transformers
- LangChain
- FAISS
- FastAPI
- Streamlit

## Project Structure

```text
evansopande61-oss-internal-medicine-expert-ai/
├── data/
├── models/
├── reports/
├── vectorstore/
├── notebooks/
├── src/
│   ├── preprocessing.py
│   ├── symptom_analyzer.py
│   ├── lab_interpreter.py
│   ├── risk_prediction.py
│   ├── clinical_summary.py
│   ├── report_generator.py
│   ├── train.py
│   ├── evaluate.py
│   └── predict.py
├── app/
│   ├── dashboard.py
│   └── api.py
├── tests/
├── requirements.txt
├── README.md
└── LICENSE
```

## Dataset

Recommended datasets:

- UCI Chronic Disease Datasets
- MIMIC-IV
- Diabetes Health Indicators Dataset
- Heart Disease Dataset
- Clinical Notes Dataset
- Lab Test Reference Dataset

## Installation

```bash
git clone https://github.com/evansopande61-oss/evansopande61-oss-internal-medicine-expert-ai.git
cd evansopande61-oss-internal-medicine-expert-ai
pip install -r requirements.txt
```

## Training Pipeline

```bash
python src/preprocessing.py
python src/train.py
python src/evaluate.py
```

## Running Prediction

```bash
python src/predict.py --input data/raw/sample_patient.json
```

Example:

```python
patient = {
    "age": 45,
    "symptoms": ["fatigue", "increased thirst", "frequent urination"],
    "fasting_glucose": 145,
    "blood_pressure": "140/90"
}

result = internal_medicine_ai.analyze(patient)

print(result["risk_level"])
print(result["possible_conditions"])
print(result["summary"])
```

## Launch Dashboard

```bash
streamlit run app/dashboard.py
```

## Run API Server

```bash
uvicorn app.api:app --reload
```

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Sensitivity
- Specificity
- Report Quality Score

## Future Improvements

- EHR integration
- Multi-disease prediction
- RAG-based medical knowledge assistant
- Lab trend monitoring
- Patient timeline analysis
- PDF clinical report export
- Voice-based patient intake
- Docker deployment

## Author

### Evans Opande

AI Engineer | Machine Learning Practitioner | Healthcare AI Enthusiast

GitHub: https://github.com/evansopande61-oss
